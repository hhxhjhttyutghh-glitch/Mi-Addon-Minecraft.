<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no, maximum-scale=1.0">
    <title>Mi RPG Pixel Art</title>
    <style>
        * {
            box-sizing: border-box;
            user-select: none;
            -webkit-user-select: none;
            -webkit-touch-callout: none;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: #000;
            overflow: hidden;
            width: 100vw;
            width: 100dvw;
            height: 100vh;
            height: 100dvh;
            position: relative;
            touch-action: none;
            font-family: sans-serif;
        }

        canvas {
            display: block;
            position: absolute;
            top: 0;
            left: 0;
            width: 100vw;
            width: 100dvw;
            height: 100vh;
            height: 100dvh;
            image-rendering: pixelated;
            image-rendering: crisp-edges;
            background-color: #2e8b57;
        }

        .menu-screen {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            width: 100dvw;
            height: 100vh;
            height: 100dvh;
            background: rgba(15, 15, 20, 0.92);
            z-index: 200;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 10px;
            overflow-y: auto;
        }

        .menu-screen.active {
            display: flex;
        }

        .game-title {
            font-size: 24px;
            font-weight: bold;
            color: #ffcc00;
            text-shadow: 2px 2px #000;
            margin-bottom: 15px;
            letter-spacing: 2px;
            text-align: center;
        }

        .menu-btn {
            width: 260px;
            max-width: 80vw;
            height: 40px;
            background: linear-gradient(to bottom, #555, #333);
            border: 2px solid #111;
            border-top: 2px solid #777;
            color: #fff;
            font-size: 13px;
            font-weight: bold;
            cursor: pointer;
            margin: 5px 0;
            text-shadow: 1px 1px #000;
            box-shadow: 0 4px 6px rgba(0,0,0,0.4);
            border-radius: 3px;
        }

        .menu-btn:active {
            background: linear-gradient(to bottom, #333, #444);
        }

        .menu-panel {
            width: 94vw;
            max-width: 580px;
            height: 85vh;
            height: 85dvh;
            max-height: 380px;
            background: #222;
            border: 3px solid #444;
            border-radius: 6px;
            display: flex;
            flex-direction: column;
            padding: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.8);
        }

        .panel-header {
            font-size: 14px;
            font-weight: bold;
            color: #fff;
            text-align: center;
            margin-bottom: 8px;
            text-shadow: 1px 1px #000;
        }

        .world-list {
            flex: 1;
            background: #111;
            border: 2px inset #333;
            border-radius: 4px;
            overflow-y: auto;
            padding: 6px;
            display: flex;
            flex-direction: column;
            gap: 5px;
        }

        .world-item {
            background: #2a2a2a;
            border: 2px solid #444;
            padding: 6px 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            cursor: pointer;
            border-radius: 4px;
            color: #fff;
        }

        .world-item.selected {
            border-color: #ffcc00;
            background: #333322;
        }

        .world-info span { display: block; }
        .world-name { font-size: 12px; font-weight: bold; color: #ffcc00; }
        .world-seed { font-size: 9px; color: #aaa; }

        .panel-footer-btns {
            display: flex;
            justify-content: space-between;
            margin-top: 8px;
            gap: 6px;
        }

        .small-btn {
            flex: 1;
            height: 34px;
            background: linear-gradient(to bottom, #555, #333);
            border: 2px solid #111;
            color: #fff;
            font-size: 11px;
            font-weight: bold;
            cursor: pointer;
            border-radius: 3px;
        }

        .form-group {
            display: flex;
            flex-direction: column;
            gap: 4px;
            margin-bottom: 10px;
        }

        .form-group label {
            font-size: 10px;
            color: #ccc;
            font-weight: bold;
        }

        .form-group input {
            background: #111;
            border: 2px solid #444;
            color: #fff;
            padding: 6px;
            font-size: 12px;
            border-radius: 3px;
            outline: none;
        }

        .option-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: #2a2a2a;
            padding: 8px;
            border-radius: 4px;
            margin-bottom: 6px;
            color: #fff;
            font-size: 11px;
        }
        .option-row input[type="range"] { width: 130px; }

        #gameUI {
            display: none;
            position: absolute;
            top: 0;
            left: 0;
            width: 100vw;
            width: 100dvw;
            height: 100vh;
            height: 100dvh;
            pointer-events: none;
            z-index: 50;
        }

        .controls-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100vw;
            width: 100dvw;
            height: 100vh;
            height: 100dvh;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 30px;
            pointer-events: none;
        }

        .btn-group {
            pointer-events: auto;
        }

        .dpad {
            display: grid;
            grid-template-columns: repeat(3, 55px);
            grid-template-rows: repeat(3, 55px);
            gap: 3px;
        }

        .action-panel {
            pointer-events: auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 8px;
        }

        .btn {
            background: transparent;
            border: none;
            border-radius: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        #up { grid-column: 2; grid-row: 1; }
        #left { grid-column: 1; grid-row: 2; }
        #right { grid-column: 3; grid-row: 2; }
        #down { grid-column: 2; grid-row: 3; }

        .dpad-btn {
            width: 55px;
            height: 55px;
            transition: filter 0.1s ease, opacity 0.1s ease;
        }

        .dpad-btn img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            pointer-events: none;
        }

        .dpad-btn.pressed {
            filter: brightness(1.4) drop-shadow(0 0 4px rgba(255,255,255,0.6));
            opacity: 0.8;
            transform: scale(0.95);
        }

        .action-btn {
            width: 75px;  
            height: 75px; 
            border-radius: 50%;
            background-color: rgba(255, 87, 34, 0.35);
            border: 2px solid #ff5722;
            color: white;
            font-size: 22px;
            font-weight: bold;
            pointer-events: auto;
            transition: background-color 0.1s ease, transform 0.1s ease;
        }

        .action-btn.pressed {
            background-color: rgba(255, 87, 34, 0.85) !important;
            border-color: #ff9800;
            transform: scale(0.92);
        }

        .interaction-btn {
            display: none;
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background-color: rgba(76, 175, 80, 0.5);
            border: 2px solid #4caf50;
            color: white;
            font-size: 18px;
            font-weight: bold;
            pointer-events: auto;
            align-items: center;
            justify-content: center;
            transition: background-color 0.1s ease, transform 0.1s ease;
        }

        .interaction-btn.pressed {
            background-color: rgba(76, 175, 80, 0.9) !important;
            border-color: #81c784;
            transform: scale(0.92);
        }

        .bottom-ui-container {
            position: fixed;
            bottom: 12px; 
            left: 50%;    
            transform: translateX(-50%);
            display: flex;
            align-items: center;
            gap: 8px;
            pointer-events: auto;
            z-index: 50;
        }

        .hotbar {
            width: 290px;
            max-width: 75vw;
            background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAAgCAYAAACy9KU0AAAB00lEQVR4AezUwW3CQBAFUMOdC33QRopOPXB1C4nmYEceLOWSjEfrF2mEbCT+7tvNv95uty/DwB1wB464A9fJHwECBA4SWAvofr9Pj8ejbPJ+5fN3/873/7cWUBTC8/n8rJjI2puK7MjYy4538V3FRNbeVGRHxl52vIvvKiayYvJUZEdGzl2e47uKWfLyZ0V2ZOTc5Tm+q5glLz43BRQvDAECBKoEFFCVtBwCBN4EFNAbiRcECFQJHFZAVRuUQ4BAXwEF1PdsrIzA8AIKaPgjtkECfQUUUN+zsbL/EvC7bQQUUJujsBAC5xNQQOc7czsm0EZAAbU5CgshcD6B8xXQ+c7Yjgm0FVBAbY/GwgiML6CAxj9jOyTQVkABtT0aCxtPwI6ygALKIp4JECgTUEBl1IIIEMgCCiiLeCZAoExAAZVRCyJAIAsooCzimQCBMgEFVEYtiACBLKCAsohnAuMJtN2RAmp7NBZGYHwBBTT+GdshgbYCCqjt0VgYgfEFFND4Z2yHBNoKbArocrl8VMzr9doFqciODPn89y5g3I2Kcf9+7t9aQPM8T5WTL0BldmTJ3wqESeVs06fSuxf7lL8VCJPKWdLXAlpe+CRAgMBfCfz2O98AAAD//0HekjkAAAAGSURBVAMAZqECeWt6X/wAAAAASUVORK5CYII=');
            background-size: 100% 100%;
            display: grid;
            grid-template-columns: repeat(9, 1fr);
            padding: 3px;
            gap: 2px;
        }

        .slot {
            width: 100%;
            aspect-ratio: 1 / 1;
            cursor: pointer;
            border-radius: 2px;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .slot img {
            width: 75%;
            height: 75%;
            object-fit: contain;
            image-rendering: pixelated;
            pointer-events: none;
        }

        .slot span {
            position: absolute;
            bottom: 1px;
            right: 2px;
            color: white;
            font-size: 9px;
            font-weight: bold;
            text-shadow: 1px 1px 0px #000;
            pointer-events: none;
        }

        .slot.active {
            border: 2px solid white;
            background-color: rgba(255, 255, 255, 0.25);
        }

        .inv-open-btn {
            width: 38px;
            height: 38px;
            background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAABhUlEQVR4AeyV3W2EQAyEL3m/Z1qhASR6oL70gEQDtMIzBRB/0RktG9vsafNzD0Qa7eIZjwdfdPd+++e/K8C1gWsDr7+Bpmm2Gpx9zYQbYPCyLB81wCMK4QagkcFRcwmHB16e1g3gNfx03QxAYkk+yjnUDsTj4bVZXmYAS5jXME6R86XPYYBHcncL8MAbRsCIpy8MgAADjHLApch5nulNNdb9NABNGOWgniLneU55734IcL/fN+CJa+t4g9RnDwDRtu0NpILoLmvuQaRJObwBs7S+B9DCNE2j3qOTFaeItMpZ3t8CqPivzqcCsO4SPBO+OACDMZa1hz9OaFTL/QyHAHxGXdf1XhPDPU7rkQZvZqiWcw+wruub/Hf28zxT/xXgzQxm6YA9AAUIwD2HvFnRj5Osf0Cb9/OMN+CuOATQondiLG8wREDj9Vt1M4CYfH0cVoO8wRjB6pHAPZ4WZwZAKEPcEPClYDhent4NQAONGNQAD7w8hAFowqAGeEQ4DRA1l3Bnmk8AAAD//9FTIu0AAAAGSURBVAMAoGR+UG4AFBsAAAAASUVORK5CYII=');
            background-size: cover;
            background-color: rgba(0,0,0,0.6);
            border: 2px solid #888;
            border-radius: 4px;
            cursor: pointer;
            flex-shrink: 0;
        }
        .inv-open-btn:active {
            transform: scale(0.95);
        }

        .pause-btn {
            position: fixed;
            top: 10px;
            right: 15px;
            width: 36px;
            height: 36px;
            background: rgba(0,0,0,0.6);
            border: 2px solid #888;
            color: white;
            font-weight: bold;
            font-size: 14px;
            border-radius: 4px;
            cursor: pointer;
            z-index: 60;
            pointer-events: auto;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .inventory-modal, .worktable-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            width: 100dvw;
            height: 100vh;
            height: 100dvh;
            background-color: rgba(0, 0, 0, 0.75);
            z-index: 100;
            pointer-events: auto;
            justify-content: center;
            align-items: center;
            padding: 4px;
        }

        .inventory-window, .worktable-window {
            width: 98vw;
            max-width: 720px;
            background-color: #c6c6c6;
            border: 4px solid #373737;
            border-radius: 6px;
            display: flex;
            padding: 8px;
            gap: 6px;
            position: relative;
            box-shadow: 0 10px 25px rgba(0,0,0,0.5);
        }

        .close-inv {
            position: absolute;
            top: 4px;
            right: 8px;
            background: #d32f2f;
            color: white;
            border: 2px solid #555;
            font-weight: bold;
            padding: 1px 6px;
            cursor: pointer;
            border-radius: 3px;
            font-size: 11px;
            z-index: 10;
        }

        .inv-col-left {
            flex: 0.7;
            display: flex;
            flex-direction: column;
            gap: 4px;
            background: #8b8b8b;
            padding: 5px;
            border: 2px solid #373737;
            border-radius: 4px;
        }
        .search-box {
            display: flex;
            align-items: center;
            background: #fff;
            border: 2px solid #373737;
            padding: 3px;
            border-radius: 3px;
        }
        .search-box input {
            border: none;
            outline: none;
            width: 100%;
            font-size: 9px;
            background: transparent;
        }
        .category-list {
            display: flex;
            flex-direction: column;
            gap: 3px;
            overflow-y: auto;
        }
        .cat-btn {
            background: #c6c6c6;
            border: 2px solid #373737;
            padding: 5px;
            font-size: 8px;
            font-weight: bold;
            cursor: pointer;
            text-align: left;
        }
        .cat-btn:active, .cat-btn.active { background: #a3a3a3; border-color: #ffeb3b; }

        .inv-col-center {
            flex: 2.9;
            display: flex;
            flex-direction: column;
            background: #8b8b8b;
            padding: 6px;
            border: 2px solid #373737;
            border-radius: 4px;
            gap: 5px;
        }

        .inv-section-title {
            font-size: 9px;
            font-weight: bold;
            color: #222;
            margin-bottom: 2px;
        }

        .inv-grid-27 {
            display: grid;
            grid-template-columns: repeat(9, 1fr);
            gap: 3px;
            width: 100%;
        }

        .inv-separator {
            width: 100%;
            height: 2px;
            background-color: #222;
            margin: 3px 0;
            border-bottom: 1px solid #555;
        }

        .inv-hotbar-grid {
            display: grid;
            grid-template-columns: repeat(9, 1fr);
            gap: 3px;
            width: 100%;
        }

        .inv-slot-item, .craft-slot, .wt-slot {
            background-color: #8b8b8b;
            border: 2px solid #373737;
            border-radius: 2px;
            width: 100%;
            aspect-ratio: 1 / 1; 
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            touch-action: none;
        }
        .inv-slot-item img, .craft-slot img, .wt-slot img, .craft-output img, .wt-output img {
            width: 75%;
            height: 75%;
            object-fit: contain;
            image-rendering: pixelated;
            pointer-events: none;
        }
        .inv-slot-item span, .craft-slot span, .wt-slot span, .craft-output span, .wt-output span {
            position: absolute;
            bottom: 1px;
            right: 2px;
            color: white;
            font-size: 9px;
            font-weight: bold;
            text-shadow: 1px 1px 0px #000;
            pointer-events: none;
        }

        .inv-slot-item.selected {
            border: 2px solid #ffeb3b !important;
            background-color: rgba(255, 235, 59, 0.3);
        }

        #cursorItem {
            display: none;
            position: fixed;
            pointer-events: none;
            z-index: 9999;
            width: 36px;
            height: 36px;
            transform: translate(-50%, -50%);
            align-items: center;
            justify-content: center;
        }
        #cursorItem img {
            width: 100%;
            height: 100%;
            object-fit: contain;
            image-rendering: pixelated;
        }
        #cursorItem span {
            position: absolute;
            bottom: 1px;
            right: 2px;
            color: white;
            font-size: 10px;
            font-weight: bold;
            text-shadow: 1px 1px 0px #000;
        }

        .inv-col-right {
            flex: 1.1;
            display: flex;
            flex-direction: column;
            gap: 5px;
            background: #8b8b8b;
            padding: 5px;
            border: 2px solid #373737;
            border-radius: 4px;
            align-items: center;
        }
        .crafting-area {
            display: flex;
            align-items: center;
            gap: 4px;
            background: #c6c6c6;
            padding: 5px;
            border: 2px solid #373737;
            border-radius: 4px;
        }
        .craft-grid-2x2 {
            display: grid;
            grid-template-columns: repeat(2, 28px);
            grid-template-rows: repeat(2, 28px);
            gap: 2px;
        }
        .craft-arrow {
            font-size: 12px;
            font-weight: bold;
            color: #373737;
        }
        .craft-output-container {
            display: flex;
            flex-direction: column;
            gap: 2px;
            align-items: center;
        }
        .craft-output {
            width: 34px;
            height: 34px;
            background: #8b8b8b;
            border: 2px solid #373737;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            cursor: pointer;
        }
        .craft-all-btn {
            width: 34px;
            height: 16px;
            background: #555;
            border: 2px solid #222;
            color: #fff;
            font-size: 7px;
            font-weight: bold;
            cursor: pointer;
            border-radius: 2px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-shadow: 1px 1px #000;
        }
        .craft-all-btn:active {
            background: #333;
        }

        .recipes-category-container {
            flex: 1;
            width: 100%;
            background: #c6c6c6;
            border: 2px solid #373737;
            padding: 4px;
            display: flex;
            flex-direction: column;
            gap: 3px;
            overflow-y: auto;
        }
        .recipe-item-row {
            display: flex;
            align-items: center;
            justify-content: space-between;
            background: #8b8b8b;
            border: 2px solid #373737;
            padding: 3px;
            cursor: pointer;
            border-radius: 3px;
        }
        .recipe-item-row:active {
            background: #666;
        }
        .recipe-item-row img {
            width: 22px;
            height: 22px;
            object-fit: contain;
            image-rendering: pixelated;
        }

        .worktable-grid-3x3 {
            display: grid;
            grid-template-columns: repeat(3, 26px);
            grid-template-rows: repeat(3, 26px);
            gap: 2px;
        }

        #customSplitModal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            background: rgba(0,0,0,0.6);
            z-index: 300;
            align-items: center;
            justify-content: center;
        }
        .split-box {
            background: #c6c6c6;
            border: 3px solid #373737;
            padding: 12px;
            border-radius: 6px;
            width: 260px;
            text-align: center;
            box-shadow: 0 8px 20px rgba(0,0,0,0.6);
        }
        .split-box h4 {
            margin: 0 0 8px 0;
            font-size: 11px;
            color: #222;
        }
        .split-input {
            width: 100%;
            background: #fff;
            border: 2px solid #373737;
            padding: 5px;
            font-size: 14px;
            font-weight: bold;
            text-align: center;
            margin-bottom: 8px;
            outline: none;
        }
        .split-quick-buttons {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 4px;
            margin-bottom: 8px;
        }
        .split-quick-buttons button {
            background: #777;
            border: 2px solid #373737;
            color: white;
            font-size: 9px;
            font-weight: bold;
            padding: 4px 0;
            cursor: pointer;
            border-radius: 2px;
        }
        .split-quick-buttons button.active {
            background: #ffcc00;
            color: #000;
            border-color: #000;
        }
        .split-actions {
            display: flex;
            gap: 6px;
        }
        .split-actions button {
            flex: 1;
            height: 30px;
            font-size: 10px;
            font-weight: bold;
            background: #8b8b8b;
            border: 2px solid #373737;
            color: white;
            cursor: pointer;
            border-radius: 3px;
        }
        .split-actions button:active { background: #555; }
    </style>
</head>
<body>

    <canvas id="gameCanvas"></canvas>
    <div id="cursorItem"></div>

    <div id="customSplitModal">
        <div class="split-box">
            <h4>SEPARAR CANTIDAD</h4>
            <input type="number" id="splitInputNumber" class="split-input" min="1" inputmode="numeric" pattern="[0-9]*">
            <div class="split-quick-buttons">
                <button id="btnDiv2" onclick="setModificadorDiv(1, 'btnDiv2')">1 Slot</button>
                <button id="btnDiv3" onclick="setModificadorDiv(2, 'btnDiv3')">x2 Slots</button>
                <button id="btnDivX2" onclick="setModificadorDiv(3, 'btnDivX2')">x3 Slots</button>
                <button id="btnDivX3" onclick="setModificadorDiv(4, 'btnDivX3')">x4 Slots</button>
            </div>
            <div class="split-actions">
                <button onclick="confirmarCustomSplit()" style="background: #2e8b57;">Aceptar</button>
                <button onclick="cerrarCustomSplitModal()" style="background: #a33;">Cancelar</button>
            </div>
        </div>
    </div>

    <!-- MESA DE TRABAJO -->
    <div class="worktable-modal" id="worktableModal">
        <div class="worktable-window">
            <button class="close-inv" onclick="toggleWorktable()">X</button>
            
            <div class="inv-col-left">
                <div class="search-box">
                    <span>🔍</span>
                    <input type="text" placeholder="Buscar...">
                </div>
                <div class="category-list">
                    <button class="cat-btn active" onclick="seleccionarCategoria('todos', 'wt')">📦 Todos</button>
                    <button class="cat-btn" onclick="seleccionarCategoria('madera', 'wt')">🪵 Madera</button>
                    <button class="cat-btn" onclick="seleccionarCategoria('tools', 'wt')">⛏️ Tools</button>
                    <button class="cat-btn" onclick="seleccionarCategoria('bloques', 'wt')">🧱 Bloques</button>
                </div>
            </div>

            <div class="inv-col-center">
                <div>
                    <div class="inv-section-title">INVENTARIO (27 SLOTS)</div>
                    <div class="inv-grid-27" id="wtInvGrid27"></div>
                </div>

                <div class="inv-separator"></div>

                <div>
                    <div class="inv-section-title">SLOTS PRINCIPALES (HOTBAR)</div>
                    <div class="inv-hotbar-grid" id="wtInvHotbarGrid"></div>
                </div>
            </div>

            <div class="inv-col-right">
                <div style="font-size: 9px; font-weight: bold; color: #373737;">MESA (3x3)</div>
                <div class="crafting-area" style="padding: 3px;">
                    <div class="worktable-grid-3x3" id="wtGrid"></div>
                    <div class="craft-arrow">➔</div>
                    <div class="craft-output-container">
                        <div class="craft-output" id="wtOutput" onclick="recolectarWorktable(false)"></div>
                        <button class="craft-all-btn" onclick="recolectarWorktable(true)">TODO</button>
                    </div>
                </div>
                <div style="font-size: 9px; font-weight: bold; color: #373737;">RECETAS RÁPIDAS</div>
                <div class="recipes-category-container" id="wtRecipesContainer"></div>
            </div>
        </div>
    </div>

    <div class="menu-screen active" id="screenMain">
        <div class="game-title">MYTHIC RPG 2D</div>
        <button class="menu-btn" onclick="abrirSelectorMundos()">JUGAR</button>
        <button class="menu-btn" onclick="abrirOpciones()">OPCIONES</button>
        <button class="menu-btn" onclick="salirJuego()">SALIR</button>
    </div>

    <div class="menu-screen" id="screenWorlds">
        <div class="menu-panel">
            <div class="panel-header">SELECCIONAR MUNDO</div>
            <div class="world-list" id="worldListContainer"></div>
            <div class="panel-footer-btns">
                <button class="small-btn" onclick="entrarMundoSeleccionado()">Jugar Mundo</button>
                <button class="small-btn" onclick="abrirCrearMundo()">Crear Nuevo</button>
                <button class="small-btn" style="background: #a33;" onclick="eliminarMundoSeleccionado()">Eliminar</button>
                <button class="small-btn" onclick="volverMenuPrincipal()">Volver</button>
            </div>
        </div>
    </div>

    <div class="menu-screen" id="screenCreateWorld">
        <div class="menu-panel" style="max-width: 450px; height: auto;">
            <div class="panel-header">CREAR NUEVO MUNDO</div>
            <div class="form-group">
                <label>NOMBRE DEL MUNDO</label>
                <input type="text" id="inputWorldName" value="Mi Aventura">
            </div>
            <div class="form-group">
                <label>SEMILLA (SEED)</label>
                <div style="display: flex; gap: 5px;">
                    <input type="text" id="inputWorldSeed" value="12345" style="flex:1;">
                    <button class="small-btn" style="width: 80px;" onclick="generarSeedAleatoria()">Aleatoria</button>
                </div>
            </div>
            <div class="panel-footer-btns">
                <button class="small-btn" style="background: #2e8b57;" onclick="crearYEntrarMundo()">¡Crear Mundo!</button>
                <button class="small-btn" onclick="abrirSelectorMundos()">Cancelar</button>
            </div>
        </div>
    </div>

    <div class="menu-screen" id="screenOptions">
        <div class="menu-panel" style="max-width: 450px; height: auto;">
            <div class="panel-header">OPCIONES</div>
            <div class="option-row">
                <span>Volumen General</span>
                <input type="range" min="0" max="100" value="80">
            </div>
            <div class="option-row">
                <span>Escala de Gráficos (Zoom)</span>
                <input type="range" min="1" max="2" step="0.1" value="1.4" id="zoomRange" oninput="cambiarZoom(this.value)">
            </div>
            <div class="panel-footer-btns" style="margin-top: 15px;">
                <button class="small-btn" onclick="volverMenuPrincipal()">Guardar y Volver</button>
            </div>
        </div>
    </div>

    <div id="gameUI">
        <button class="pause-btn" onclick="pausarJuego()">⏸</button>

        <div class="controls-overlay">
            <div class="btn-group dpad">
                <div></div>
                <div class="btn dpad-btn" id="up"><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACdUlEQVR4AeybQXaDMAxESY/BoXLYHIprtAwvcgzBtmRLAlz6ouJYsjXzxaKb/gzfP7/zVs8x2/t8tgBg/JPtc7XyGANYJcZxHHqKzSyDVwIQNlAI43hO0/TqIeCFPGH9jsUzACyL9+YydaxhHM8egrzsQQCA4BEFKEaETfvF077FMMATAh7jfgEAEiiIkw5rMk9P85bwCK/UKACgjf/2PBLAdurb7y6zOArAIWb3iB4FYE8L9tzBHAGgZLKUByi1OAKAmniNi7wBcKfLrWtm4AnAzZSEiicAiS7UmgDDxXF4Aag1U3su9phdewAwN5F1WEh6AChIKKZNAVoDMBVfRMcosAbAkMAqMQNpCUBbtPZ9C3krACZiF8XKv6wAKMsM16mDtQCgLjLYN1hoA/Awr9pDG4DBjHavVIOgCUBN1K5lo01NAEYSk9eqANcCoCImaTWdaO6rAaBZRNqffUYDgL3KfIfsAPJHh6EVQFPzkjiPfAuAM5mv1tICwGNAkh5VEGoBVDWTuPGqrQXgpU/aRzyYGgDiJlIXnvVSAFcwL9IoBeA5nJZebAgSAOxLW5R7n+UCuKJ5lmYuAO/BuPXjAGCRdFMsa1TUzgEga3m+6iyEEoDs4fN5lSvKAejJfNJLDoAc5wlOSCWkACSJSRucqH7XUwrAaxbeY8y21p8UgHVVx99uAB0Pl2XtfgNYmDouut+AjofLsna/AYRpmib8x9juX0tU08NzHMcnvJKX1RuABAoQVNDLE54Q8Bh7AoBHvEEFKI73r7wmL+Qt8vIAAHxPQsDhqwcM7pnHPgHA+gsCDvUSMBhF8BoDQD4k8OUKUaFx5fEPAAD//yPJN7oAAAAGSURBVAMAFY8SZ5DuFFYAAAAASUVORK5CYII=" alt="Up"></div>
                <div></div>
                <div class="btn dpad-btn" id="left"><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACaElEQVR4AdyZUXarMAwF2y6DRXWxWRTbSDM55zqghBQcbEt6591KxjZopp/9+Xr+d709ypwb3uO/FQD4Yzdnt2JcClhtTNP0lSnmd1lYJaA84CDg8zxfMgUm2Ba5MyPg3miDg4BrnaXCBJvhuSKgPHtxoOw5bn6PzGYZiwBtYOrICweeBZzsHkFsYuViEcBCB+gdB2hSNaJlXAmoemPfS9XgW2NGEQA42eKofu5dANCkGvC/i54FNAWXGI8CACeasWn1JABo0hTYvtyLgO7gEjFaAOBE8zSv9gOjBABN7Dzd1yMEuACX6Z4CACf6tovaS4A7cNlvLQBwou+5q60EAE3cAduBWggIAS4RZwoAnOjdIeoZAoAmIYDtkJ8KCAsuEbUCACd6T9h6VADQJCywHfyIgFTgErFHAOBEd1LVdwKAJqmALcyWgDTgFtiutwRc7MGs6y0B8CKB0KfNOwGCTi1hjwBEIIHQp8peAYJGAtE6fD0qQMBpJNQKQAQSCH3YfCJA0KElnCEAEUgg9KFylgBBI4Fo7b6eLUDAYSS0EoAIJBB6t2kpQNCuJfQQgAgkEHpX6SVA0EggWg+vvQUIuJkEfWBvHSWA+ZBA6IdlpABBD5XgQQAikEDou8aLAEEjgWjdvHoTIOBuErwKQAQSCH2zeBYg6KYSIghABBII/amJIkDQSCBaf1xXAqZpivIXoWoJlrEImOf5btMeuD/0+QMJZPd0YhMrF4sAFssN1kFySIJlRMD3EpQDMrV8Hr2HCTbD8Y0Anr2UwKUseQUPuATQP0ngUpYAuEhhXQpgv2ywiJCKGVeMfwAAAP//2fFx/gAAAAZJREFUAwCeQwhngi6wkwAAAABJRU5ErkJggg==" alt="Left"></div>
                <div></div>
                <div class="btn dpad-btn" id="right"><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACb0lEQVR4AeSZ7XGDMBAFScqgqBTromjDYZl5spCxMQJJp3PGL3f6wNxufuZ3eP65z1ueM+M9PqkAwB+nPrsVYyxgdTCO4+Apyd8ysEpA2OAi4NM03TwFJtiiLMwIWBodcBFwrb1UmGBLeO4ICHsbF8LZi+bvxb7Z7ZQxCNABpg5OjwRy8LH618UmViYIAljoAn1GupIgvpUAbZ6oSCAnvqLuo1cL0PRIIFqbraUECNi8hNICEIEEQm8uNQQI2qSEmgIQgQRCbyK1BQgaCUTrZrWVAAFXl6AXq7YWwBxIIPTVY0GAoJtIsCQAEUgg9FViTYCgkUC0LlatChBwcQnWBSACCYT+8vQgQNBFJPQkABFIIPSXpDcBgkYC0Tq79ipAwKcl9C4AEUgg9IfjQYCgsyR4EoAIJBD6j+JNgKCRQLR+Wb0KEPCuBO8ChtkEEsjcPn++QYCoNyV8k4CbTMT1GwQATmLu0HsWADQJsFuNVwG74JLhTQDgRHy71YsAoMkucHrBg4AscInoWQDgRCxZtUcBQJMs4PSh3gRcBi4RvQgAnGjuy6p1AUCTy4DTL7IsoCi4RFgUADjRjEWrNQGnwY/asiIAcHJ0/tP3WwsAmpwGyf2ClgKagktYCwGAE83QtNYUADRpCpy+vJYAc+ASUVoA4ETvM1dLCQCamANOByohoAtwiVgJGMdx858HurxTASc719oep4xBwDRNy2TphWXz/S+gyftbBk7FJlZGCgJYxAesP0gX4DFHyoiAn/SCTMX7vfcwpfAz0w8C5jpsSuAhL9mCB1wC6J8k8JCXABglsMYCOA8HLHpIxowrxn8AAAD//9ZYt30AAAAGSURBVAMAppAIZzh+67QAAAAASUVORK5CYII=" alt="Right"></div>
                <div></div>
                <div class="btn dpad-btn" id="down"><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACaElEQVR4AeybXXaDIBBG0y7DRWWxWZTbaHNzAkEiCuMwItrTOSK/37342P7evn/+nl091xPv8xsLAPwz2mdrwhgKmAwMw3DrqaK79KxOgO9gIuA8x3F89FCwOCba73oxI+DVeHe+bp024Dx7KMcyJwEBnpEJTKZ8ZycNmCgYQyQvgAEmhIM9tmGE1bF5Aa7jbM9LwNluPOa9voDYyNnery/gbDce815fQGzk/X5/Pnus25Nr8pv6Ah6TWX28zDKlBPSBnEGxJGDWWMaeLU5JsiwJaBFEkikJz2ZrAhYXs8HRa00AfEeWsJo9RwASuq1cAasmGzSUlTlXQIN8i5Gy4NmhRED2pmx8lCoRANMRJBRlLBWAhJarCB4QiYDiQzio1ZIIaJVFdDFSAaLDWjQnFQBLSxKSWQi6VFsELO1rOSaGJ+RWAZsOJ8DetVXA3vk3X4CGgM0hhBZVztUQQH6VMGxkXVoCrHOrCdcUoBbK0qamAHJbSFA9Q1sAEmqWKjxBawhQD0nQWlVDQK2sVcTWEqAdVns/f0m1BHBAtdBsrlU1BWhlrCqytoCq4TUM1xawNWOxwNIDLQRIIaTrihxYCCCQCQwHlZaVgNJcZsIsBeRC5c4rlTo731LAbIC9O60FrN3u2ri6L2sBAJhDcmiq9hCQyrKLmL0ExLDxe0qSev9eAtRBpBt6AeM48h9j/HmsdK/Sde7W3bN0vWj+MAx3WN1iL4AOBphA8W5QZvAwUTCGXAj4CTvcBCaH/UduOxbHFrD8IID3pAQWH70AnIOn3wmg/SWBRb0UgEF51lAA436AlyOUIOOE8R8AAP//M8566wAAAAZJREFUAwCsWxJnehSIqgAAAABJRU5ErkJggg==" alt="Down"></div>
                <div></div>
            </div>

            <div class="action-panel">
                <div class="btn action-btn" id="actionBtn">A</div>
                <div class="btn interaction-btn" id="interactBtn">🛠️</div>
            </div>
        </div>

        <div class="bottom-ui-container">
            <div class="hotbar" id="hotbar">
                <div class="slot active" onclick="seleccionarSlot(0)"></div>
                <div class="slot" onclick="seleccionarSlot(1)"></div>
                <div class="slot" onclick="seleccionarSlot(2)"></div>
                <div class="slot" onclick="seleccionarSlot(3)"></div>
                <div class="slot" onclick="seleccionarSlot(4)"></div>
                <div class="slot" onclick="seleccionarSlot(5)"></div>
                <div class="slot" onclick="seleccionarSlot(6)"></div>
                <div class="slot" onclick="seleccionarSlot(7)"></div>
                <div class="slot" onclick="seleccionarSlot(8)"></div>
            </div>
            <div class="inv-open-btn" onclick="toggleInventario()"></div>
        </div>
    </div>

    <!-- INVENTARIO PRINCIPAL -->
    <div class="inventory-modal" id="invModal">
        <div class="inventory-window" id="invWindow">
            <button class="close-inv" onclick="toggleInventario()">X</button>
            
            <div class="inv-col-left">
                <div class="search-box">
                    <span>🔍</span>
                    <input type="text" placeholder="Buscar...">
                </div>
                <div class="category-list">
                    <button class="cat-btn active" onclick="seleccionarCategoria('todos', 'inv')">📦 Todos</button>
                    <button class="cat-btn" onclick="seleccionarCategoria('madera', 'inv')">🪵 Madera</button>
                    <button class="cat-btn" onclick="seleccionarCategoria('tools', 'inv')">⛏️ Tools</button>
                    <button class="cat-btn" onclick="seleccionarCategoria('bloques', 'inv')">🧱 Bloques</button>
                </div>
            </div>

            <div class="inv-col-center">
                <div>
                    <div class="inv-section-title">INVENTARIO (27 SLOTS)</div>
                    <div class="inv-grid-27" id="invGrid27"></div>
                </div>

                <div class="inv-separator"></div>

                <div>
                    <div class="inv-section-title">SLOTS PRINCIPALES (HOTBAR)</div>
                    <div class="inv-hotbar-grid" id="invHotbarGrid"></div>
                </div>
            </div>

            <div class="inv-col-right">
                <div style="font-size: 9px; font-weight: bold; color: #373737;">CRAFTEO (2x2)</div>
                <div class="crafting-area">
                    <div class="craft-grid-2x2" id="craftGrid"></div>
                    <div class="craft-arrow">➔</div>
                    <div class="craft-output-container">
                        <div class="craft-output" id="craftOutput" onclick="recolectarCrafting(false)"></div>
                        <button class="craft-all-btn" onclick="recolectarCrafting(true)">TODO</button>
                    </div>
                </div>
                <div style="font-size: 9px; font-weight: bold; color: #373737;">RECETAS RÁPIDAS</div>
                <div class="recipes-category-container" id="invRecipesContainer"></div>
            </div>
        </div>
    </div>

    <script>
const TEXTURAS_EMBEBIDAS = {
  "abajo": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACaElEQVR4AeybXXaDIBBG0y7DRWWxWZTbaHNzAkEiCuMwItrTOSK/37342P7evn/+nl091xPv8xsLAPwz2mdrwhgKmAwMw3DrqaK79KxOgO9gIuA8x3F89FCwOCba73oxI+DVeHe+bp024Dx7KMcyJwEBnpEJTKZ8ZycNmCgYQyQvgAEmhIM9tmGE1bF5Aa7jbM9LwNluPOa9voDYyNnery/gbDce815fQGzk/X5/Pnus25Nr8pv6Ah6TWX28zDKlBPSBnEGxJGDWWMaeLU5JsiwJaBFEkikJz2ZrAhYXs8HRa00AfEeWsJo9RwASuq1cAasmGzSUlTlXQIN8i5Gy4NmhRED2pmx8lCoRANMRJBRlLBWAhJarCB4QiYDiQzio1ZIIaJVFdDFSAaLDWjQnFQBLSxKSWQi6VFsELO1rOSaGJ+RWAZsOJ8DetVXA3vk3X4CGgM0hhBZVztUQQH6VMGxkXVoCrHOrCdcUoBbK0qamAHJbSFA9Q1sAEmqWKjxBawhQD0nQWlVDQK2sVcTWEqAdVns/f0m1BHBAtdBsrlU1BWhlrCqytoCq4TUM1xawNWOxwNIDLQRIIaTrihxYCCCQCQwHlZaVgNJcZsIsBeRC5c4rlTo731LAbIC9O60FrN3u2ri6L2sBAJhDcmiq9hCQyrKLmL0ExLDxe0qSev9eAtRBpBt6AeM48h9j/HmsdK/Sde7W3bN0vWj+MAx3WN1iL4AOBphA8W5QZvAwUTCGXAj4CTvcBCaH/UduOxbHFrD8IID3pAQWH70AnIOn3wmg/SWBRb0UgEF51lAA436AlyOUIOOE8R8AAP//M8566wAAAAZJREFUAwCsWxJnehSIqgAAAABJRU5ErkJggg==",
  "acha": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAACp0lEQVR4AcSWT0tUYRTGz5UklJxSSyiFiSDa9R3aCu3cRS3aRLQJwk21Capdy4igRSCCC9d+F3eOG0Hxv+hGuJ7f0fNyZhxnrnPvRbnPnPOe+855nnPeP86Q3PBf1QJyrQeoKfZUKSD/8WFW5t+8gLmwiKoEGPnE3VG5NzaCgAjERMR3MtQ2Gmxg5Hz1wfgdQcSfz3MMjXTh+yuJ0BfE1Zw/ZQUk8mePp2Rr90gQcZ5ahCVZ39j1YVdbRkB+sd5WNeQwrK5tYoz8y+8V83uJKCPA1vv500dye/iWEcXq6Qgd6CeijICM5C8//rO2I4IusAdQg4+NIl5/XSSU8eEoI4AcJMsQwQDs7B9jBEsXGAQRzCeUUFZASoRDF7CQ0wn2A5YYItRyAiKqO4Zvvy1pfpGH9xtm4wciwMrfTxKhc/KyHbCTsHd4YrseEWxEF+FLQEzJpNVqyfHBNm5CGQHpDvDbjzazHyBkOXwjuk2swRlUQKo85DI3imAvEEQQwO/EIAKMnERUDlgCxoCjqdZOxvTMtLpiN6R34eh02GKz735hs+sKaCMnA5sLEfhOjg+mJhp2R3j1I2PjQox3jusIMHLIgCfAIqKTnDgYbUwKVTebzUTu1fO+qIC04fiSA2L89z+XMZcuGYLAq4YYaCzNLSLAKmedY+UFyDPIIi6IE7mO+15ERs5EJ4cYEOtXuc6BLEJD7U+vDqS2R3L/egFyn9rTXiXAyGPbvWqyVUVOrm4CEjkTQF3k5I4C7L8UNxkvuqHKyj2/C7CqIec8U3HnutdBjggE5PyKhZQAIiBj/GRmkpAwVofdrKbaBwF2XZIWUqyLwK+TnPwmAMfv6y4iaqkcTpAEMOgUQaxuICCbm/+feFwEm1GDtVav+dNVbCIQAqpcd0h64QwAAP//HIHDvwAAAAZJREFUAwBfDfg9qdnAbQAAAABJRU5ErkJggg==",
  "arbol": "data:image/png;base64,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",
  "arriba": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACdUlEQVR4AeybQXaDMAxESY/BoXLYHIprtAwvcgzBtmRLAlz6ouJYsjXzxaKb/gzfP7/zVs8x2/t8tgBg/JPtc7XyGANYJcZxHHqKzSyDVwIQNlAI43hO0/TqIeCFPGH9jsUzACyL9+YydaxhHM8egrzsQQCA4BEFKEaETfvF077FMMATAh7jfgEAEiiIkw5rMk9P85bwCK/UKACgjf/2PBLAdurb7y6zOArAIWb3iB4FYE8L9tzBHAGgZLKUByi1OAKAmniNi7wBcKfLrWtm4AnAzZSEiicAiS7UmgDDxXF4Aag1U3su9phdewAwN5F1WEh6AChIKKZNAVoDMBVfRMcosAbAkMAqMQNpCUBbtPZ9C3krACZiF8XKv6wAKMsM16mDtQCgLjLYN1hoA/Awr9pDG4DBjHavVIOgCUBN1K5lo01NAEYSk9eqANcCoCImaTWdaO6rAaBZRNqffUYDgL3KfIfsAPJHh6EVQFPzkjiPfAuAM5mv1tICwGNAkh5VEGoBVDWTuPGqrQXgpU/aRzyYGgDiJlIXnvVSAFcwL9IoBeA5nJZebAgSAOxLW5R7n+UCuKJ5lmYuAO/BuPXjAGCRdFMsa1TUzgEga3m+6iyEEoDs4fN5lSvKAejJfNJLDoAc5wlOSCWkACSJSRucqH7XUwrAaxbeY8y21p8UgHVVx99uAB0Pl2XtfgNYmDouut+AjofLsna/AYRpmib8x9juX0tU08NzHMcnvJKX1RuABAoQVNDLE54Q8Bh7AoBHvEEFKI73r7wmL+Qt8vIAAHxPQsDhqwcM7pnHPgHA+gsCDvUSMBhF8BoDQD4k8OUKUaFx5fEPAAD//yPJN7oAAAAGSURBVAMAFY8SZ5DuFFYAAAAASUVORK5CYII=",
  "derecha": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACb0lEQVR4AeSZ7XGDMBAFScqgqBTromjDYZl5spCxMQJJp3PGL3f6wNxufuZ3eP65z1ueM+M9PqkAwB+nPrsVYyxgdTCO4+Apyd8ysEpA2OAi4NM03TwFJtiiLMwIWBodcBFwrb1UmGBLeO4ICHsbF8LZi+bvxb7Z7ZQxCNABpg5OjwRy8LH618UmViYIAljoAn1GupIgvpUAbZ6oSCAnvqLuo1cL0PRIIFqbraUECNi8hNICEIEEQm8uNQQI2qSEmgIQgQRCbyK1BQgaCUTrZrWVAAFXl6AXq7YWwBxIIPTVY0GAoJtIsCQAEUgg9FViTYCgkUC0LlatChBwcQnWBSACCYT+8vQgQNBFJPQkABFIIPSXpDcBgkYC0Tq79ipAwKcl9C4AEUgg9IfjQYCgsyR4EoAIJBD6j+JNgKCRQLR+Wb0KEPCuBO8ChtkEEsjcPn++QYCoNyV8k4CbTMT1GwQATmLu0HsWADQJsFuNVwG74JLhTQDgRHy71YsAoMkucHrBg4AscInoWQDgRCxZtUcBQJMs4PSh3gRcBi4RvQgAnGjuy6p1AUCTy4DTL7IsoCi4RFgUADjRjEWrNQGnwY/asiIAcHJ0/tP3WwsAmpwGyf2ClgKagktYCwGAE83QtNYUADRpCpy+vJYAc+ASUVoA4ETvM1dLCQCamANOByohoAtwiVgJGMdx858HurxTASc719oep4xBwDRNy2TphWXz/S+gyftbBk7FJlZGCgJYxAesP0gX4DFHyoiAn/SCTMX7vfcwpfAz0w8C5jpsSuAhL9mCB1wC6J8k8JCXABglsMYCOA8HLHpIxowrxn8AAAD//9ZYt30AAAAGSURBVAMAppAIZzh+67QAAAAASUVORK5CYII=",
  "inventario_btn": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAABhUlEQVR4AeyV3W2EQAyEL3m/Z1qhASR6oL70gEQDtMIzBRB/0RktG9vsafNzD0Qa7eIZjwdfdPd+++e/K8C1gWsDr7+Bpmm2Gpx9zYQbYPCyLB81wCMK4QagkcFRcwmHB16e1g3gNfx03QxAYkk+yjnUDsTj4bVZXmYAS5jXME6R86XPYYBHcncL8MAbRsCIpy8MgAADjHLApch5nulNNdb9NABNGOWgniLneU55734IcL/fN+CJa+t4g9RnDwDRtu0NpILoLmvuQaRJObwBs7S+B9DCNE2j3qOTFaeItMpZ3t8CqPivzqcCsO4SPBO+OACDMZa1hz9OaFTL/QyHAHxGXdf1XhPDPU7rkQZvZqiWcw+wruub/Hf28zxT/xXgzQxm6YA9AAUIwD2HvFnRj5Osf0Cb9/OMN+CuOATQondiLG8wREDj9Vt1M4CYfH0cVoO8wRjB6pHAPZ4WZwZAKEPcEPClYDhent4NQAONGNQAD7w8hAFowqAGeEQ4DRA1l3Bnmk8AAAD//9FTIu0AAAAGSURBVAMAoGR+UG4AFBsAAAAASUVORK5CYII=",
  "izquierda": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAACaElEQVR4AdyZUXarMAwF2y6DRXWxWRTbSDM55zqghBQcbEt6591KxjZopp/9+Xr+d709ypwb3uO/FQD4Yzdnt2JcClhtTNP0lSnmd1lYJaA84CDg8zxfMgUm2Ba5MyPg3miDg4BrnaXCBJvhuSKgPHtxoOw5bn6PzGYZiwBtYOrICweeBZzsHkFsYuViEcBCB+gdB2hSNaJlXAmoemPfS9XgW2NGEQA42eKofu5dANCkGvC/i54FNAWXGI8CACeasWn1JABo0hTYvtyLgO7gEjFaAOBE8zSv9gOjBABN7Dzd1yMEuACX6Z4CACf6tovaS4A7cNlvLQBwou+5q60EAE3cAduBWggIAS4RZwoAnOjdIeoZAoAmIYDtkJ8KCAsuEbUCACd6T9h6VADQJCywHfyIgFTgErFHAOBEd1LVdwKAJqmALcyWgDTgFtiutwRc7MGs6y0B8CKB0KfNOwGCTi1hjwBEIIHQp8peAYJGAtE6fD0qQMBpJNQKQAQSCH3YfCJA0KElnCEAEUgg9KFylgBBI4Fo7b6eLUDAYSS0EoAIJBB6t2kpQNCuJfQQgAgkEHpX6SVA0EggWg+vvQUIuJkEfWBvHSWA+ZBA6IdlpABBD5XgQQAikEDou8aLAEEjgWjdvHoTIOBuErwKQAQSCH2zeBYg6KYSIghABBII/amJIkDQSCBaf1xXAqZpivIXoWoJlrEImOf5btMeuD/0+QMJZPd0YhMrF4sAFssN1kFySIJlRMD3EpQDMrV8Hr2HCTbD8Y0Anr2UwKUseQUPuATQP0ngUpYAuEhhXQpgv2ywiJCKGVeMfwAAAP//2fFx/gAAAAZJREFUAwCeQwhngi6wkwAAAABJRU5ErkJggg==",
  "madera_procesada": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAACHUlEQVR4AezVvU5UURTF8SO1xhijFlrZ2dr7BpY+gLGzsLSzNDaW9sYHoPQN7K1IaAgVhAAhhEAP+ZEscuZyP2fuhAaSlb3PPfvs/9rnMjMb5Y7/7g2s7QZ2/367HPN212IA/P/2XhGHTMxuYPPnx0vwgIdMzGoAHPjtm1flxdNHZf/o7Fr/fn/pfB2zGcik4MCMvHz+uJC8y8SGzVUFnmsHByU56X94cl5yQ9bRygbA08y1A1sHLAe3J2+aWMlA4KYH6IMzwQDVr2NpA+DAVMMBmgJXQ/beffr1QKSlDASuIdWT5+pBCUTN1s5Bsf7w9c8N3N5kA95hptaghlsTEKicwJ89eViacHuTDJjcIc2ByTpTywMXrY9PL0oX3P5oA+CZPGAN+uD2++D2RxnItfuScSiq4Z65mXpy07ddu9po0AB4imtgnQcqgpLJP//YXPiHS5869hoI3OSmy9UHDqiZPXnA4EOTO0edBmo4ILjoEAECJxeBxbFwta0G2uCKI3C5SHLTi1Pg6m8ZaIObnBwIUB6o3PRT4c4tGADP+wZsu3aHcvWg1rQM3LkFA2kCTEwoonpyuemjnFM3VQsGHH79/vv1R6cJNzUFanoa81HTt0u3DCiMCblpRZKDymmVyZ2nVgM26p9Mk4N7TkzMAder04BNJppwz+eC69VrQAETYjQnXM9BA4oCTfRsLo0yALYOuL6jDSheRkNnrgAAAP//v+WNwgAAAAZJREFUAwA2s2hQYnU8AQAAAABJRU5ErkJggg==",
  "mesa_trabajo": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAACOElEQVR4AexVu05bQRAdOyTKQ4kSpUiTEgXxCfmI9KnS5HtSpqRJlbRRuiRCggIJIeQKLARCRiDES+Zl2XBlmz0XZj13dpblWhgakM+dc2bnca4XQZXu+efBwMM3YH0Dffd7OUq48YOPNtD//+0LjRJEhJdz4fKjDVCj0aD5Wt0jpduHu1QGl2sHz8AAHx22zpnmMaXzoiEeUQOvXzwpjEvpQnEJYRp49+YZMTCLOaKlkRsWVatxp9kmBs6ZI1oauanV98SA1tg9ahOg86YBFKXuXJ+jJwZrMddGDaTuXJ9/Hd+kickJQuThWAywtqJpAHfNQBNzREsjJ4GlgMwdnHQIkDlw0wDumoEi5ohaYxHjw/6f4J6tpZjBMA3gcGPvlOQ9pzR6ACwEwBnQb18+ZVmIpgEsfvV88HfgOo3hEjydc1IzlzEw8P13jf4trnuk9M/pOpWBXA4eGEDyLhEY+PRxnEYJ/XJVnThy/4Qk9HlZLWeB6/7AgCxYWVoiNAGdyc+eyxrJUScxM1eTxya/1kCrW/FNZws/PJdLJPcFV6RbeXTF4iEwcNzOiEH9quecKxOJekG/thIYkAU94w1OO5ks8dzK92nMn8eINlCZ+lsnYH55i5rZGCECyAG/Ztfyc3AJnUdPM3sc9Dsjg3t1QhtwKSoUICGAs5tAtBQoegsJy0BekHV7BORiyAf6GbERUQPckBrAdTqiT+csnTRgNd1mLmagUt9ukYRbGtyfy8U+vp9nuEKz/wIAAP//rDarRQAAAAZJREFUAwBHXHBXDzdhnwAAAABJRU5ErkJggg==",
  "palo": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAABLElEQVR4AeSWsQrCMBRFo5uCKH6dv+A3uDi5OLs6ODu7+idOrooiKIqgnCElraZNXvPqYOHS0jbvnKQJTdv8+PgvgeV09LKxA9/YCAAGen88DeGaNCLgwoG6URcogyOiKuCDj2frFnCiJhACVxMIhasIxMCTC8TCkwpI4MkEpPAkAt/gx/PVuEsNkC+1lqEPPllssnXuA9v7YoEUcCREAqngIoGU8GiBIpzJRmK+OVA3wZ/gG5xCdeC0DxLQggcJaMIrBbThpQJNwL0CRTgvkroTjhrFfExCC7cvssyIBhxGTsDC2TaT3f5ghv2u0YLnBFw4D+j1oNcJ/qvRRpLcCNBrigDnrNlz6pNMwIWfLjfVYQdskwmwgSD0er7aBv/PbSHpOROQFqhqV/X8DQAA//9PDxsJAAAABklEQVQDAOWy/UEx0B7sAAAAAElFTkSuQmCC",
  "pasto": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAL9klEQVR4ASSXWXMb6XWGn96wr8RCAAS4ShQpUSONlpmMMslkMnGlUpVKfkXs/IK4KkvlKinf5CYXTqryF+KLXLoc2+NZLWu0DaUZSiIJccdK7ECjG92fD2ncob8+y/ee9z3ntK7//TW1/F931cZ/b6nIP6wo7UfrKv1vd1TkX5bVn//sjxU/vKbm/+OmWv/pdRX7xzXFjzZU/id3VeDHS+rj/32gtB9eV8s/va82/2dLBX+8ojQ5z/37PRX71z/Ya3+3eWm/8p/XVfifly7Psz+5r0L/tKw++dmfKl0pxVImTvPUJBrOUFhN4vs+kVAUK5zDNHwMFaTZC5KMZVi8lmIm59FUhEAwC5rLUj5Gdc8mHc6KfRTX97BC4ctzI+CiK5PhJMJcLM/CtbT4nxGJRMR3Rs6UjeuEGPUHuLMpDkMMb0o4ZvHFL6rMrUZRExPlgDJ98Exs25FkdX7+f9+hLBvPiTKbuHhBj8lkgunbcm7y6S/3SC3HYRJiMpxy8dMxmE498R/kV5++Qv/LH1T46uvvSKRThDIGN5Yq3LxV4uhFk9G4Du6QuVKAUX2CYXZZroTQ9S7HO32YdvnkT8p88ZvnZPMZLN3l9kaF61vzHL/sYE86Yj8gVTSZNKfogZ6gHQXV4+RlE7fTRn960COeSTD0xpwft2lPhjz5skFwPkQ4FaJx6tLqdjBSLqcnLs2+I3fIEEhr5LfyfFvtkyym6TsjWqddaoLkk9+1CBYDhJMBeebSFnszPePsyKbpTdBGSTnXKW7l0MOWgXJnoGuCQom9N3UqNyI4XY0bWyWsqEZ9pwNSg1wmxVG1RbkS58G9VaaTAGYwgNsfoek6wXiGg2qT8pUo08aMaxs5tLBG802PcMiiWMhxIP6Xb8d5f2uZ/hD0s2OHRDaC4TtcECoRytBqCrwzj6OjU9JJwFKkkmEWywkS0STVoxP2jnqM7AndWoe5Shp95hOSYInQHO3OQDyb1M7aZOZ0dFMRDmiUy3FS8QRvd+vsnY7wpwrd7foSwefBexWU5lNcENirYxbWE0yEXFev3SC/ImrwdHaqdQi5jE8VvqaYtUdMzo1LVj+4VZGgispaWG48YWkzhT0LsX71OnPlDNpM8fTJAXpEZ9hwUEoI25+KCjSoH9v8+usq3WaP51/vUVzO4og6bt3M89tf7zPuuwTiPv3WmMZxj/xyhk7rnA//YllKY1A7sfnlkx1acvbN5zsUr86JGgbc3BD7r/aZeh6GpYl8Fae7bXLltNh3+OiTIvrS9bjISJFIpNFMj9J6UaTloXwDe6zhuVPu3ihwcqgoLeRZu1Vg4jrkSjn8WZhLXbs+qaSglISFchlPeoOQg+HIwxdZ3lrL02h55AoZrt6eF2Q88uLL8yLotppIdjbtgyEZYfN6ZZ5g2BCYFNtvaqxvFHm1cy69ISiEUuT1CBfNa9xz2P6+AeYIM+zK7QekUinWNwtSb4vO0ZSXew3W1uZ5I/aaaxCOGRQCcQR3xp0JT5820ZHaGMJkPWigSV196VwTqY09HDDrOzQaLZr9Pq4gcYGKAMMHd8p0zhwcu4/CxTRNQc/ACs5w1ZTx1MHtj2EKtWadeq+HJ2W4eK6EkO+uleg25F2vKyR0fJyWTTxrMTzt8fBZFSugo2ZBQcaFmEV5IS26N6i/OeHLT6s8f33CbDYkMR8WXljYYp/MBmjt9vjd4300NZOEIgSEaMFUnKWVrDQ5i/pujc9/tcfrWh13MCKTSaM7ozAXkHTPhmQKi9y/s8rJ9wOSi0l80xJ9e/QEDUyNhZUVPvyrCp3mAJTBaiGPYRjgK7oiy6Lc7M7dNRq7NulSkmnAA21Gt9vF1xWVlSt8/Der0tx6YHlUpJ/oyYxHMB0FW6Bz+5y8HnHxc7pTInoUmSt4cqPZTOKYDrvftglFpI6C0PazfcJRn0AiAjOX4WhMbbeP1JKR1DhiJvGkxC4+SojqGhP2Xl7Yx9C8KN+9OECfC2cwwwalzQLTcZ+LSXbhIJQy6J31CblhLtgednVxA6XCPJViDDOiWJbJmAgkCCR1yjcWmNojPB9JxiM6J/Zv2wSNmCgpQGBmygzRyc9nWFqIoVszKgtJ9O0nJywvZkknDEYDn+O9Jql8hM7hKR//dYn62YBo0hTt6rRrbZ7KrXtDl9mwTyKYEIY3KRdy0iHBmTgcHzRILyc5P6nx0d8u0qh2iIl9oWzQOmnw+OFbhkNQaiQxJRFMyGUC7H7XZy6VISNZ+bpBZXOVbjtELB7E1EzpAx759DxLV7I40xlX7l4R9sdQuivPg+zvDEnF86SLCXyRXOXaMoNOQOxDWATY352QmcuxspnBdqYs31zCCCXQCytRHn29z0Ixy3m3w1UZIAvFOL5m8/1uDSulc340JjYXpDceUmu05Uxqqo354rPXZIshnjypXpam2W3JAMpTKIRRmsPOTuMP9gcjYqKYsUzMQxlGmu4jpODz/99Bv7kawVM+dRlAd+6VCQmpK9k4pztd7ElPGtqQezLzu4dTaSRT7m1VqBQM9p4NwJhy+3oKR1RQP+ty951lqTmsFpOcvukwHndkK5rw3kerDA49QmHFB++vUs4Z7L8YX9rrD78dXXaw2JzJ9uO37Jwc8fDFCSHR9ebNCs1XGlWpXe6KxfnZmP36CcevDEJ5l9X1Mg+f98nmkoTmfLa3D3i1f8yXT4+wxN/1e4vUdzzenh6TXtM4P+2y1zjl7VmAYGzKmhBXz5Z8cqk5ycYRopXADRKJz7DbHrlEiNRShHZtgnIc3vtgE584fnLEvRurjDybfClKJpwSpHwKSyV8M0g4NWPaVPI8fLnSNc5sLEHp3oMtlMjP9zv8kSAxsR3005e+GE2xBwNJQgzPNdGujmZYfPtyn1RkRjBq4krvd12bScshbFnU2kPcsSndrYUKunjTqfSjqQT20D2Di993r/eJhfxLe0fsL96Z9FyisRC18yHjriRgT6Yow+OD21ex2y4bUtPzQ5vrtzIk0nmWri1JHSUhYfKr53XyKwHqB2ORkUDarjPsGFz0+VvrS+JwyDvvFmhVXbbu54nH51m8UiIYtLC0CC+f1JibtyTpMb7sF91eH11DkzWsz+PtKiPH5uFnO6RESq3zOrlckIe/OJEG4xPJeAyGY5r7MzLFFO1Gi83NOJIJ+7IXvtjbYzxUMiu+JbUQvxxihYUQjz47Yyorn5Uc4wQc4YFHppzk7LTFxrUYenErgZL2ZURCAqHD4s0yKytJPC3AbKpj20PuS5es1QzyC/PkrxhSHjCjYTLJMuV3U3IFD4wIZkyxuLzC6moKzzDp1x2mwxHv36jQ6oRIJrLkV3XJWRQRD5IrLqJ3WyOUzM3aW5t0NsFKLkP1sE5zb8D3r1p8+Gc3ePT4GCsUZGY5zMcSlwnb4wFffX5A97wp/10ahxMJEKaymOD1myPa+0PZ+3q89/4mD5+8lU1aAutTMlYEdIOBcODzn++ix2KmfPHECeghYgld1vKJzARNoAXNd3m+vYMZMSWIQyET5pWM3Hc3MqhRgljaIyxkjQh6AStOMATnIxtvFhBjD3c44fXhK8yLQuu+NKsoeydD3t3IYrkJojkdfdxStOTbIFawOHhRY0+2mIthh7KE2WPi2RjzCxGU7rG7fcjFTZ/tnTHpt3BtxXgSlOVkSDQ142z/nGr1nHDcBycsI3hCMp2mUIkh6fBa+kNDCPx051B4cQ5Sen1mKsnW57zeYWVtgzvvLFHfPWf1nUUpq1zJgH5vQjRhsbpyg49lwPRkq5UQ3Lm/jj8FfLEXWebnFrl7tyTNp8OSfF0ZAslFlx0MxkTiJsvrV3nwg5IMIxd36nPr1jX0UjnGnLBS10zOGnUe/ea1jNe4rGBCrImJJQlICJl0EjI85ptHVXQzIEFjPPtmm/xSjOxKRm4j5ZMV7dFnVYLpGI7sF5YTkHJ7wjF5faYJilOePz4V6QVhFuXFs5dy7lpoQUU6qYgkIF/JyIrmollj8AIYk6gE18WJgyMfHwvzBa6uJ9F0l5u3VzDcgHTHGfmShc6YuUKMaVsJaT2mIx/TjmGPdFHTWNZPV3aALCuybUm34tY7a/weAAD//7fjVpEAAAAGSURBVAMA+PXxL+DJCbgAAAAASUVORK5CYII=",
  "personaje_abajo": "data:image/png;base64,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",
  "personaje_arriba": "data:image/png;base64,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",
  "personaje_derecha": "data:image/png;base64,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",
  "personaje_izquierda": "data:image/png;base64,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",
  "slot": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAASAAAAAgCAYAAACy9KU0AAAB00lEQVR4AezUwW3CQBAFUMOdC33QRopOPXB1C4nmYEceLOWSjEfrF2mEbCT+7tvNv95uty/DwB1wB464A9fJHwECBA4SWAvofr9Pj8ejbPJ+5fN3/873/7cWUBTC8/n8rJjI2puK7MjYy4538V3FRNbeVGRHxl52vIvvKiayYvJUZEdGzl2e47uKWfLyZ0V2ZOTc5Tm+q5glLz43BRQvDAECBKoEFFCVtBwCBN4EFNAbiRcECFQJHFZAVRuUQ4BAXwEF1PdsrIzA8AIKaPgjtkECfQUUUN+zsbL/EvC7bQQUUJujsBAC5xNQQOc7czsm0EZAAbU5CgshcD6B8xXQ+c7Yjgm0FVBAbY/GwgiML6CAxj9jOyTQVkABtT0aCxtPwI6ygALKIp4JECgTUEBl1IIIEMgCCiiLeCZAoExAAZVRCyJAIAsooCzimQCBMgEFVEYtiACBLKCAsohnAuMJtN2RAmp7NBZGYHwBBTT+GdshgbYCCqjt0VgYgfEFFND4Z2yHBNoKbArocrl8VMzr9doFqciODPn89y5g3I2Kcf9+7t9aQPM8T5WTL0BldmTJ3wqESeVs06fSuxf7lL8VCJPKWdLXAlpe+CRAgMBfCfz2O98AAAD//0HekjkAAAAGSURBVAMAZqECeWt6X/wAAAAASUVORK5CYII=",
  "tronco": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAADZUlEQVR4AdyVT0hUURTGz4jknzQbpCmppMgoISg0yAwK2qQUUUQLIYSgVm3atBHatomgTbsgaiMU0UaRoMSCpoJGIiSVlLJMa0RsGNGMYLq/E/d15zHT/PFF4PC+e+4999z7fefc9+6UyH/+rVgBKVPYTDDu9OdfVCD1+FqngJ7LbQKunt0nXaf3iPkhypg/T9AClHzxW1wANMOTcxhpqKsRhJhBmoggBXjkhkQgjo58kdrqcgW+TAhKgEcOMYCMrLEu/FUIQkCKc4aEjLFu1rHxGZlNfpex6YR8iCcVxFgsV4BmHq5vlMGhUQlXlaWVG9KaylWWS61/vBwBSl6+plai0agSk7mymAZyY1QUNhuKFaDkbGrJ6Vv4yefmlySx8EPI/sq914SFaEAxAjxyyu5mzYZ+cnyQYzkirItCBXgvHN85mbmbZSK3MVsi1XLp1kvCvewZFCJAM69YG9FLhk/N/cwgJ0PAxgByss9GTkwJTR5QcuLIHHK39JaceYt8yInNR0DB5GxM5rx0mcrOvEUuAR75xMSEXq/+zO1G1rqXjf+NtzGuzSaAPwwlp+TALuJWo0/ZsfbMLTFZgxu9b5lOe+Fw+JFJQKrz8HYBt3ufy91n4xJPLOq6F6NxvXB0YBqX3Ay9J5/MbbBfAJnr3P6W3XK8/YBge199lIGhKTm6t17naPgCEETfRSHkrHMFpE61bpX25s1KvKuhTtbXVsu6cJVcPHdMzp9pUxEsQhDYEK7QPxdKjj/fshNrYQVo2TtOHpKuCyd07utsUgAicAyNTaswKtGyIyIAP+CNL4actSU0LjZGaqSpcZMCcsaAiszMzasIN55Lplhy9kGAlp7zxgG6+wYFPI2Ny+d4Qh5GR7QaR1p3CiL630wRpn8uub5zDfxLgwCdJls6EB5s3iYd7U0MPTCPECphnYW+cHada1XA6vJS4YzdCSrAmPJjXVSWlWb8Y3Fj8u2rAILJjCytEKoAqAjzVsj1mz0MAwMCQnf634ndmHNGhAXEiEPIo4GY3I++VxgFOW85E5PzQYAGLSz9VGvPGVLugMHhSfUjSDu/m0DI2coKCPXFPmkVyJLv3yWkOvjJ3iwKjNzsJVYA/RAEoPvBE4EQC/ABExQoudkvTQBjCDwhkAIzoX5jC35yLfgFAAD//2x9TSYAAAAGSURBVAMAdu22TJT501gAAAAASUVORK5CYII="
};
const IMAGENES_CACHE = {};
for (const [k, v] of Object.entries(TEXTURAS_EMBEBIDAS)) {
    const img = new Image();
    img.src = v;
    IMAGENES_CACHE[k] = img;
}

        const canvas = document.getElementById("gameCanvas");
        const ctx = canvas.getContext("2d");
        ctx.imageSmoothingEnabled = false;

        function resizeCanvas() {
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
        }
        window.addEventListener('resize', resizeCanvas);
        resizeCanvas();

        const pastoImg = new Image(); pastoImg.src = "data:image/png;base64,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";
        const arbolImg = new Image(); arbolImg.src = "data:image/png;base64,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";
        const imgAbajo = new Image(); imgAbajo.src = "data:image/png;base64,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";
        const imgArriba = new Image(); imgArriba.src = "data:image/png;base64,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";
        const imgIzquierda = new Image(); imgIzquierda.src = "data:image/png;base64,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";
        const imgDerecha = new Image(); imgDerecha.src = "data:image/png;base64,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";

        let ultimaDireccion = 'abajo';
        let frameAnimacion = 0;
        let contadorPasos = 0;

        let gameState = 'MENU'; 
        let mundosGuardados = JSON.parse(localStorage.getItem('rpg_mundos') || '[]');
        let mundoSeleccionadoIndex = 0;
        let mundoActual = null;
        let zoomGlobal = 1.4;

        let player = { x: 2000, y: 2000, size: 40, speed: 1.5 };

        let hotbar = Array(9).fill(null).map(() => ({ item: null, cantidad: 0 }));
        let inventarioStorage = Array(27).fill(null).map(() => ({ item: null, cantidad: 0 }));
        let craftingGrid = Array(4).fill(null).map(() => ({ item: null, cantidad: 0 }));
        let worktableGrid = Array(9).fill(null).map(() => ({ item: null, cantidad: 0 }));
        let slotActivo = 0;

        let itemSeleccionado = null; 
        let pressTimer = null;
        let splitTarget = null;
        let multiplicadorSlots = 1;
        let isHolding = false;

        let categoriaActivaInv = 'todos';
        let categoriaActivaWt = 'todos';

        let seedActual = 12345;
        let arbolesDestruidos = new Set();
        let arbolesEstado = {};
        let arbolesAnimaciones = {};
        let itemsEnSuelo = []; 
        let mesasEnMundo = []; 
        let ultimoGolpeTiempo = 0;

        function getMaxStack(itemNombre) { 
            if (itemNombre === 'acha') return 1;
            return 64; 
        }

        // Helper para comprobar si un ítem es tronco/madera cortada
        function esMaderaEnBruto(item) {
            return item === 'tronco' || item === 'madera';
        }

        function cambiarPantalla(pantallaId) {
            document.querySelectorAll('.menu-screen').forEach(s => s.classList.remove('active'));
            document.getElementById('gameUI').style.display = 'none';
            
            if (pantallaId === 'game') {
                document.getElementById('gameUI').style.display = 'block';
                gameState = 'PLAYING';
            } else {
                document.getElementById(pantallaId).classList.add('active');
                gameState = pantallaId.toUpperCase();
            }
        }

        function volverMenuPrincipal() { cambiarPantalla('screenMain'); }
        function abrirOpciones() { cambiarPantalla('screenOptions'); }
        function abrirCrearMundo() { cambiarPantalla('screenCreateWorld'); }
        function salirJuego() { alert("Puedes cerrar esta pestaña o app."); }

        function abrirSelectorMundos() {
            actualizarListaMundosUI();
            cambiarPantalla('screenWorlds');
        }

        function generarSeedAleatoria() {
            document.getElementById('inputWorldSeed').value = Math.floor(Math.random() * 1000000);
        }

        function actualizarListaMundosUI() {
            const container = document.getElementById('worldListContainer');
            container.innerHTML = '';
            if (mundosGuardados.length === 0) {
                container.innerHTML = `<div style="color: #888; text-align: center; padding: 20px; font-size: 11px;">No hay mundos creados. ¡Crea uno nuevo!</div>`;
                return;
            }
            mundosGuardados.forEach((m, idx) => {
                let div = document.createElement('div');
                div.className = `world-item ${idx === mundoSeleccionadoIndex ? 'selected' : ''}`;
                div.onclick = () => { mundoSeleccionadoIndex = idx; actualizarListaMundosUI(); };
                div.innerHTML = `
                    <div class="world-info">
                        <span class="world-name">🗺️ ${m.nombre}</span>
                        <span class="world-seed">Semilla: ${m.seed} | Jugado: ${m.fecha}</span>
                    </div>
                `;
                container.appendChild(div);
            });
        }

        function crearYEntrarMundo() {
            let nombre = document.getElementById('inputWorldName').value || "Mi Aventura";
            let seed = parseInt(document.getElementById('inputWorldSeed').value) || 12345;
            
            let nuevoMundo = {
                nombre: nombre,
                seed: seed,
                fecha: new Date().toLocaleDateString(),
                playerX: 2000,
                playerY: 2000,
                hotbar: Array(9).fill(null).map(() => ({ item: null, cantidad: 0 })),
                storage: Array(27).fill(null).map(() => ({ item: null, cantidad: 0 })),
                arbolesDestruidos: [], arbolesEstado: {}, itemsEnSuelo: [], mesasEnMundo: []
            };

            mundosGuardados.push(nuevoMundo);
            localStorage.setItem('rpg_mundos', JSON.stringify(mundosGuardados));
            mundoSeleccionadoIndex = mundosGuardados.length - 1;
            entrarMundoSeleccionado();
        }

        function eliminarMundoSeleccionado() {
            if (mundosGuardados.length === 0) return;
            if (confirm("¿Estás seguro de eliminar este mundo permanentemente?")) {
                mundosGuardados.splice(mundoSeleccionadoIndex, 1);
                localStorage.setItem('rpg_mundos', JSON.stringify(mundosGuardados));
                mundoSeleccionadoIndex = 0;
                actualizarListaMundosUI();
            }
        }

        function entrarMundoSeleccionado() {
            if (mundosGuardados.length === 0) { abrirCrearMundo(); return; }
            mundoActual = mundosGuardados[mundoSeleccionadoIndex];
            seedActual = mundoActual.seed;
            player.x = mundoActual.playerX;
            player.y = mundoActual.playerY;
            hotbar = mundoActual.hotbar;
            inventarioStorage = mundoActual.storage;
            arbolesDestruidos = new Set(mundoActual.arbolesDestruidos || []);
            arbolesEstado = mundoActual.arbolesEstado || {};
            itemsEnSuelo = mundoActual.itemsEnSuelo || [];
            mesasEnMundo = mundoActual.mesasEnMundo || [];
            arbolesAnimaciones = {};

            cambiarPantalla('game');
            actualizarInventariosVisuales();
        }

        function pausarJuego() {
            if (mundoActual) {
                mundoActual.playerX = player.x; mundoActual.playerY = player.y;
                mundoActual.hotbar = hotbar; mundoActual.storage = inventarioStorage;
                mundoActual.arbolesDestruidos = Array.from(arbolesDestruidos);
                mundoActual.arbolesEstado = arbolesEstado;
                mundoActual.itemsEnSuelo = itemsEnSuelo;
                mundoActual.mesasEnMundo = mesasEnMundo;
                localStorage.setItem('rpg_mundos', JSON.stringify(mundosGuardados));
            }
            abrirSelectorMundos();
        }

        function cambiarZoom(val) { zoomGlobal = parseFloat(val); }

        window.addEventListener('pointermove', (e) => {
            let clientX = e.clientX || (e.touches && e.touches[0].clientX) || e.pageX;
            let clientY = e.clientY || (e.touches && e.touches[0].clientY) || e.pageY;
            
            const cursorDiv = document.getElementById('cursorItem');
            if (cursorDiv) {
                cursorDiv.style.left = clientX + 'px';
                cursorDiv.style.top = clientY + 'px';
            }
        });

        window.addEventListener('pointerup', () => {
            if (pressTimer) { clearTimeout(pressTimer); pressTimer = null; }
            isHolding = false;
        });

        function pseudoRandom(x, y) {
            let n = Math.sin(x * 12.9898 + y * 78.233 + seedActual) * 43758.5453;
            return n - Math.floor(n);
        }

        function getArbolesCercanos() {
            let lista = [];
            let chunkSize = 400;
            let playerChunkX = Math.floor(player.x / chunkSize);
            let playerChunkY = Math.floor(player.y / chunkSize);
            let radius = 2;

            for (let cx = playerChunkX - radius; cx <= playerChunkX + radius; cx++) {
                for (let cy = playerChunkY - radius; cy <= playerChunkY + radius; cy++) {
                    for (let i = 0; i < 5; i++) {
                        let rx = pseudoRandom(cx * 100 + i, cy * 100);
                        let ry = pseudoRandom(cx * 100, cy * 100 + i);
                        let treeX = cx * chunkSize + rx * (chunkSize - 50);
                        let treeY = cy * chunkSize + ry * (chunkSize - 50);
                        let treeId = `${cx},${cy},${i}`;

                        if (!arbolesDestruidos.has(treeId)) {
                            if (arbolesEstado[treeId] === undefined) arbolesEstado[treeId] = 15;
                            lista.push({ key: treeId, x: treeX, y: treeY, width: 64, height: 96, hp: arbolesEstado[treeId] });
                        }
                    }
                }
            }
            return lista;
        }

        let keys = { up: false, down: false, left: false, right: false };

        function setupBtn(id, keyName) {
            const btn = document.getElementById(id);
            if (!btn) return;
            const pressOn = (e) => { e.preventDefault(); keys[keyName] = true; btn.classList.add('pressed'); };
            const pressOff = (e) => { keys[keyName] = false; btn.classList.remove('pressed'); };
            btn.addEventListener("touchstart", pressOn, { passive: false });
            btn.addEventListener("touchend", pressOff, { passive: true });
            btn.addEventListener("touchcancel", pressOff, { passive: true });
            btn.addEventListener("mousedown", () => { keys[keyName] = true; btn.classList.add('pressed'); });
            btn.addEventListener("mouseup", () => { keys[keyName] = false; btn.classList.remove('pressed'); });
            btn.addEventListener("mouseleave", () => { keys[keyName] = false; btn.classList.remove('pressed'); });
        }

        setupBtn("up", "up"); setupBtn("down", "down"); setupBtn("left", "left"); setupBtn("right", "right");

        const actionBtn = document.getElementById("actionBtn");
        const actionOn = (e) => { e.preventDefault(); actionBtn.classList.add('pressed'); ejecutarGolpeA(); };
        const actionOff = () => { actionBtn.classList.remove('pressed'); };
        actionBtn.addEventListener("touchstart", actionOn, { passive: false });
        actionBtn.addEventListener("touchend", actionOff, { passive: true });
        actionBtn.addEventListener("touchcancel", actionOff, { passive: true });
        actionBtn.addEventListener("mousedown", () => { actionBtn.classList.add('pressed'); ejecutarGolpeA(); });
        actionBtn.addEventListener("mouseup", actionOff);
        actionBtn.addEventListener("mouseleave", actionOff);

        const interactBtn = document.getElementById("interactBtn");
        const interactOn = (e) => { e.preventDefault(); interactBtn.classList.add('pressed'); toggleWorktable(); };
        const interactOff = () => { interactBtn.classList.remove('pressed'); };
        interactBtn.addEventListener("touchstart", interactOn, { passive: false });
        interactBtn.addEventListener("touchend", interactOff, { passive: true });
        interactBtn.addEventListener("touchcancel", interactOff, { passive: true });
        interactBtn.addEventListener("mousedown", () => { interactBtn.classList.add('pressed'); toggleWorktable(); });
        interactBtn.addEventListener("mouseup", interactOff);
        interactBtn.addEventListener("mouseleave", interactOff);

        function ejecutarGolpeA() {
            if (gameState !== 'PLAYING') return;
            let ahora = Date.now();
            if (ahora - ultimoGolpeTiempo < 180) return;
            ultimoGolpeTiempo = ahora;

            let pX = player.x + player.size / 2;
            let pY = player.y + player.size / 2;

            let mesaCercana = null, menorDistMesa = 65, idxMesa = -1;
            for (let i = 0; i < mesasEnMundo.length; i++) {
                let m = mesasEnMundo[i];
                let dist = Math.hypot(pX - (m.x + 12.5), pY - (m.y + 12.5));
                if (dist < menorDistMesa) { menorDistMesa = dist; mesaCercana = m; idxMesa = i; }
            }

            if (mesaCercana) {
                let danioMesa = 1;
                let itemMano = hotbar[slotActivo];
                if (itemMano && itemMano.item === 'acha' && itemMano.cantidad > 0) {
                    danioMesa = Math.ceil(8 / 8); 
                }
                mesaCercana.hp -= danioMesa;
                if (mesaCercana.hp <= 0) {
                    devolverGridAlInventario(worktableGrid);
                    agregarAlInventario('mesa_trabajo', 1);
                    mesasEnMundo.splice(idxMesa, 1);
                }
                return;
            }

            let arbolesVisibles = getArbolesCercanos();
            let arbolMasCercano = null, menorDistancia = 70;
            for (let a of arbolesVisibles) {
                let distancia = Math.hypot((player.x + player.size/2) - (a.x + a.width/2), (player.y + player.size/2) - (a.y + a.height/2));
                if (distancia < menorDistancia) { menorDistancia = distancia; arbolMasCercano = a; }
            }

            if (arbolMasCercano) {
                let a = arbolMasCercano;
                if (arbolesAnimaciones[a.key] && arbolesAnimaciones[a.key].breaking) return;

                let danioGolpe = 1;
                let itemMano = hotbar[slotActivo];
                if (itemMano && itemMano.item === 'acha' && itemMano.cantidad > 0) {
                    danioGolpe = Math.ceil(15 / 8);
                }

                arbolesEstado[a.key] -= danioGolpe;
                arbolesAnimaciones[a.key] = { shake: 12, breaking: false };

                if (arbolesEstado[a.key] <= 0) {
                    arbolesAnimaciones[a.key] = { shake: 0, breaking: true, breakTimer: 15 };
                    setTimeout(() => {
                        if (!arbolesDestruidos.has(a.key)) {
                            arbolesDestruidos.add(a.key);
                            itemsEnSuelo.push({ id: Date.now() + Math.random(), item: 'tronco', cantidad: 2, x: a.x + a.width / 2 - 12, y: a.y + a.height - 25 });
                        }
                    }, 250);
                }
            }
        }

        function devolverItemAlInventario(itemNombre, cantidad, forzarNuevoSlot = false) {
            if (!itemNombre || cantidad <= 0) return;
            let maxStack = getMaxStack(itemNombre);

            if (!forzarNuevoSlot) {
                for (let i = 0; i < hotbar.length; i++) {
                    if (hotbar[i].item === itemNombre && hotbar[i].cantidad < maxStack) {
                        let espacio = maxStack - hotbar[i].cantidad;
                        let aSumar = Math.min(espacio, cantidad);
                        hotbar[i].cantidad += aSumar; cantidad -= aSumar;
                        if (cantidad <= 0) return;
                    }
                }
                for (let i = 0; i < inventarioStorage.length; i++) {
                    if (inventarioStorage[i].item === itemNombre && inventarioStorage[i].cantidad < maxStack) {
                        let espacio = maxStack - inventarioStorage[i].cantidad;
                        let aSumar = Math.min(espacio, cantidad);
                        inventarioStorage[i].cantidad += aSumar; cantidad -= aSumar;
                        if (cantidad <= 0) return;
                    }
                }
            }

            for (let i = 0; i < inventarioStorage.length; i++) {
                if (inventarioStorage[i].item === null || inventarioStorage[i].cantidad <= 0) {
                    let aSumar = Math.min(maxStack, cantidad);
                    inventarioStorage[i] = { item: itemNombre, cantidad: aSumar }; cantidad -= aSumar;
                    if (cantidad <= 0) return;
                }
            }
            for (let i = 0; i < hotbar.length; i++) {
                if (hotbar[i].item === null || hotbar[i].cantidad <= 0) {
                    let aSumar = Math.min(maxStack, cantidad);
                    hotbar[i] = { item: itemNombre, cantidad: aSumar }; cantidad -= aSumar;
                    if (cantidad <= 0) return;
                }
            }

            if (cantidad > 0) itemsEnSuelo.push({ id: Date.now() + Math.random(), item: itemNombre, cantidad: cantidad, x: player.x, y: player.y });
        }

        function devolverGridAlInventario(grid) {
            for (let i = 0; i < grid.length; i++) {
                if (grid[i].item !== null && grid[i].cantidad > 0) {
                    devolverItemAlInventario(grid[i].item, grid[i].cantidad);
                    grid[i] = { item: null, cantidad: 0 };
                }
            }
        }

        function rescatarItemCursor() {
            if (itemSeleccionado !== null) {
                let itemNombre = null, itemCantidad = 0;
                if (itemSeleccionado.item !== undefined && itemSeleccionado.tipo === undefined) {
                    itemNombre = itemSeleccionado.item; itemCantidad = itemSeleccionado.cantidad;
                } else if (itemSeleccionado.tipo !== undefined) {
                    let arr;
                    if (itemSeleccionado.tipo === 'storage') arr = inventarioStorage;
                    else if (itemSeleccionado.tipo === 'hotbar') arr = hotbar;
                    else if (itemSeleccionado.tipo === 'craft') arr = craftingGrid;
                    else if (itemSeleccionado.tipo === 'wt') arr = worktableGrid;

                    let slotObj = arr ? arr[itemSeleccionado.index] : null;
                    if (slotObj && slotObj.item) {
                        itemNombre = slotObj.item; itemCantidad = slotObj.cantidad;
                        arr[itemSeleccionado.index] = { item: null, cantidad: 0 };
                    }
                }
                if (itemNombre && itemCantidad > 0) devolverItemAlInventario(itemNombre, itemCantidad);
                itemSeleccionado = null;
            }
        }

        function agregarAlInventario(itemNombre, cantidad) {
            devolverItemAlInventario(itemNombre, cantidad);
            actualizarInventariosVisuales();
        }

        let ultimoToqueSlot = { tipo: null, index: -1, tiempo: 0 };

        function manejarClickSlot(tipo, index) {
            let inventarioActual;
            if (tipo === 'storage') inventarioActual = inventarioStorage;
            else if (tipo === 'hotbar') inventarioActual = hotbar;
            else if (tipo === 'craft') inventarioActual = craftingGrid;
            else if (tipo === 'wt') inventarioActual = worktableGrid;
            else return;

            let slotObj = inventarioActual[index];
            let ahora = Date.now();

            if (ultimoToqueSlot.tipo === tipo && ultimoToqueSlot.index === index && (ahora - ultimoToqueSlot.tiempo) < 500) {
                if (slotObj.item !== null && itemSeleccionado === null) {
                    unirTodosLosItemsEnSlotDestino(tipo, index, slotObj.item);
                    ultimoToqueSlot = { tipo: null, index: -1, tiempo: 0 };
                    actualizarInventariosVisuales();
                    return;
                }
            }
            ultimoToqueSlot = { tipo, index, tiempo: ahora };

            if (itemSeleccionado === null) {
                if (slotObj.item !== null) { itemSeleccionado = { tipo, index }; actualizarInventariosVisuales(); }
            } else {
                if (itemSeleccionado.item !== undefined && itemSeleccionado.tipo === undefined) {
                    let destinoItem = inventarioActual[index];
                    let maxStack = getMaxStack(itemSeleccionado.item);

                    if (destinoItem.item === null) {
                        let aPoner = Math.min(maxStack, itemSeleccionado.cantidad);
                        inventarioActual[index] = { item: itemSeleccionado.item, cantidad: aPoner };
                        itemSeleccionado.cantidad -= aPoner;
                        if (itemSeleccionado.cantidad <= 0) itemSeleccionado = null;
                    } else if (destinoItem.item === itemSeleccionado.item && maxStack > 1) {
                        let espacio = maxStack - destinoItem.cantidad;
                        let aSumar = Math.min(espacio, itemSeleccionado.cantidad);
                        destinoItem.cantidad += aSumar;
                        itemSeleccionado.cantidad -= aSumar;
                        if (itemSeleccionado.cantidad <= 0) itemSeleccionado = null;
                    } else {
                        let temp = { ...destinoItem };
                        inventarioActual[index] = { item: itemSeleccionado.item, cantidad: itemSeleccionado.cantidad };
                        itemSeleccionado = { item: temp.item, cantidad: temp.cantidad };
                    }
                } else {
                    let origenArray;
                    if (itemSeleccionado.tipo === 'storage') origenArray = inventarioStorage;
                    else if (itemSeleccionado.tipo === 'hotbar') origenArray = hotbar;
                    else if (itemSeleccionado.tipo === 'craft') origenArray = craftingGrid;
                    else if (itemSeleccionado.tipo === 'wt') origenArray = worktableGrid;

                    let origenIndex = itemSeleccionado.index;
                    if (itemSeleccionado.tipo === tipo && origenIndex === index) {
                        itemSeleccionado = null; actualizarInventariosVisuales(); return;
                    }

                    let origenItem = origenArray[origenIndex];
                    let destinoItem = inventarioActual[index];
                    let maxStack = getMaxStack(origenItem.item);

                    if (destinoItem.item === origenItem.item && destinoItem.item !== null && maxStack > 1) {
                        let espacio = maxStack - destinoItem.cantidad;
                        let aSumar = Math.min(espacio, origenItem.cantidad);
                        destinoItem.cantidad += aSumar; origenItem.cantidad -= aSumar;
                        if (origenItem.cantidad <= 0) origenArray[origenIndex] = { item: null, cantidad: 0 };
                    } else {
                        let temp = { ...origenItem };
                        origenArray[origenIndex] = { ...destinoItem };
                        inventarioActual[index] = temp;
                    }
                    itemSeleccionado = null;
                }
                actualizarInventariosVisuales();
            }
        }

        function unirTodosLosItemsEnSlotDestino(tipoDestino, indexDestino, itemNombre) {
            let maxStack = getMaxStack(itemNombre);
            if (maxStack === 1) return;

            let invDest;
            if (tipoDestino === 'storage') invDest = inventarioStorage;
            else if (tipoDestino === 'hotbar') invDest = hotbar;
            else if (tipoDestino === 'craft') invDest = craftingGrid;
            else if (tipoDestino === 'wt') invDest = worktableGrid;

            let slotDest = invDest[indexDestino];
            let cantidadAcumulada = slotDest.cantidad;
            slotDest.item = null; slotDest.cantidad = 0;

            let todasLasGrids = [hotbar, inventarioStorage, craftingGrid, worktableGrid];
            todasLasGrids.forEach(g => {
                g.forEach(s => {
                    if (s.item === itemNombre) { cantidadAcumulada += s.cantidad; s.item = null; s.cantidad = 0; }
                });
            });

            slotDest.item = itemNombre;
            let aPoner = Math.min(maxStack, cantidadAcumulada);
            slotDest.cantidad = aPoner;
            cantidadAcumulada -= aPoner;
            if (cantidadAcumulada > 0) devolverItemAlInventario(itemNombre, cantidadAcumulada);
        }

        function handleSlotDown(tipo, index) {
            isHolding = true;
            pressTimer = setTimeout(() => {
                if (isHolding) { pressTimer = null; abrirCustomSplitModal(tipo, index); }
            }, 1000);
        }

        function handleSlotUp(tipo, index) {
            isHolding = false;
            if (pressTimer) { clearTimeout(pressTimer); pressTimer = null; }
            let modalInv = document.getElementById('invModal').style.display === 'flex';
            let modalWt = document.getElementById('worktableModal').style.display === 'flex';
            if (tipo === 'hotbar' && !modalInv && !modalWt) seleccionarSlot(index);
            manejarClickSlot(tipo, index);
        }

        function setModificadorDiv(num, btnId) {
            multiplicadorSlots = num;
            ['btnDiv2', 'btnDiv3', 'btnDivX2', 'btnDivX3'].forEach(id => {
                let b = document.getElementById(id);
                if (b) b.classList.remove('active');
            });
            let bSel = document.getElementById(btnId);
            if (bSel) bSel.classList.add('active');
        }

        function abrirCustomSplitModal(tipo, index) {
            splitTarget = { tipo, index };
            let inv;
            if (tipo === 'storage') inv = inventarioStorage;
            else if (tipo === 'hotbar') inv = hotbar;
            else if (tipo === 'craft') inv = craftingGrid;
            else if (tipo === 'wt') inv = worktableGrid;

            let slot = inv ? inv[index] : null;
            if (!slot || slot.cantidad <= 1 || getMaxStack(slot.item) === 1) return;

            setModificadorDiv(1, 'btnDiv2');
            const inputNum = document.getElementById('splitInputNumber');
            inputNum.value = Math.floor(slot.cantidad / 2);
            document.getElementById('customSplitModal').style.display = 'flex';
            setTimeout(() => { inputNum.focus(); inputNum.select(); }, 100);
        }

        function cerrarCustomSplitModal() {
            document.getElementById('customSplitModal').style.display = 'none';
            splitTarget = null;
        }

        function confirmarCustomSplit() {
            if (!splitTarget) return;
            const inputNum = document.getElementById('splitInputNumber');
            let porcionDeseada = parseInt(inputNum.value);

            let inv;
            if (splitTarget.tipo === 'storage') inv = inventarioStorage;
            else if (splitTarget.tipo === 'hotbar') inv = hotbar;
            else if (splitTarget.tipo === 'craft') inv = craftingGrid;
            else if (splitTarget.tipo === 'wt') inv = worktableGrid;

            let slot = inv ? inv[splitTarget.index] : null;
            if (!slot) return;

            let totalARetirar = porcionDeseada * multiplicadorSlots;

            if (isNaN(porcionDeseada) || porcionDeseada <= 0 || totalARetirar > slot.cantidad) {
                alert(`No tienes suficiente cantidad en el slot para crear ${multiplicadorSlots} pilas de ${porcionDeseada} (Requiere ${totalARetirar}).`);
                return;
            }

            slot.cantidad -= totalARetirar;
            let itemNombre = slot.item;
            if (slot.cantidad <= 0) { slot.item = null; slot.cantidad = 0; }

            cerrarCustomSplitModal();
            // Colocar cada una de las divisiones en slots libres e independientes
            for (let k = 0; k < multiplicadorSlots; k++) {
                devolverItemAlInventario(itemNombre, porcionDeseada, true);
            }
            actualizarInventariosVisuales();
        }

        function seleccionarCategoria(cat, ventana) {
            if (ventana === 'inv') categoriaActivaInv = cat;
            else categoriaActivaWt = cat;
            actualizarInventariosVisuales();
        }

        function renderizarRecetasRapidas(containerId, ventana) {
            const container = document.getElementById(containerId);
            if (!container) return;
            container.innerHTML = '';

            let cat = (ventana === 'inv') ? categoriaActivaInv : categoriaActivaWt;
            let recetasDisponibles = [];

            if (cat === 'todos' || cat === 'madera' || cat === 'tools') {
                recetasDisponibles.push({ resultado: 'madera_procesada', cantidad: 3, nombre: '3x Madera' });
                recetasDisponibles.push({ resultado: 'palo', cantidad: 4, nombre: '4x Palo' });
                recetasDisponibles.push({ resultado: 'mesa_trabajo', cantidad: 1, nombre: 'Mesa de Trabajo' });
                if (ventana === 'wt') {
                    recetasDisponibles.push({ resultado: 'acha', cantidad: 1, nombre: 'Hacha de Madera' });
                }
            }

            if (recetasDisponibles.length === 0) {
                container.innerHTML = `<div style="font-size: 8px; color: #333; text-align: center; padding: 10px;">No hay recetas en esta categoría.</div>`;
                return;
            }

            recetasDisponibles.forEach(receta => {
                let row = document.createElement('div');
                row.className = 'recipe-item-row';
                row.onclick = () => craftearRecetaRapida(receta);
                row.innerHTML = `
                    <div style="display: flex; align-items: center; gap: 4px;">
                        <img src="${TEXTURAS_EMBEBIDAS[receta.resultado] || ""}">
                        <span style="font-size: 8px; font-weight: bold; color: #222;">${receta.nombre}</span>
                    </div>
                    <span style="font-size: 8px; font-weight: bold; color: #005500;">➔ Craftear</span>
                `;
                container.appendChild(row);
            });
        }

        function craftearRecetaRapida(receta) {
            if (receta.resultado === 'madera_procesada') {
                let encontrado = false;
                for (let i = 0; i < inventarioStorage.length; i++) {
                    if (esMaderaEnBruto(inventarioStorage[i].item) && inventarioStorage[i].cantidad > 0) {
                        inventarioStorage[i].cantidad--;
                        if (inventarioStorage[i].cantidad <= 0) inventarioStorage[i] = { item: null, cantidad: 0 };
                        encontrado = true; break;
                    }
                }
                if (!encontrado) {
                    for (let i = 0; i < hotbar.length; i++) {
                        if (esMaderaEnBruto(hotbar[i].item) && hotbar[i].cantidad > 0) {
                            hotbar[i].cantidad--;
                            if (hotbar[i].cantidad <= 0) hotbar[i] = { item: null, cantidad: 0 };
                            encontrado = true; break;
                        }
                    }
                }
                if (encontrado) agregarAlInventario('madera_procesada', receta.cantidad);
                else alert("No tienes troncos para craftear madera.");
            } else if (receta.resultado === 'palo') {
                let encontrado = false;
                for (let i = 0; i < inventarioStorage.length; i++) {
                    if (inventarioStorage[i].item === 'madera_procesada' && inventarioStorage[i].cantidad > 0) {
                        inventarioStorage[i].cantidad--;
                        if (inventarioStorage[i].cantidad <= 0) inventarioStorage[i] = { item: null, cantidad: 0 };
                        encontrado = true; break;
                    }
                }
                if (!encontrado) {
                    for (let i = 0; i < hotbar.length; i++) {
                        if (hotbar[i].item === 'madera_procesada' && hotbar[i].cantidad > 0) {
                            hotbar[i].cantidad--;
                            if (hotbar[i].cantidad <= 0) hotbar[i] = { item: null, cantidad: 0 };
                            encontrado = true; break;
                        }
                    }
                }
                if (encontrado) agregarAlInventario('palo', 4);
                else alert("Necesitas madera procesada para hacer palos.");
            } else if (receta.resultado === 'mesa_trabajo') {
                let maderasNecesarias = 4, encontradas = 0, slotsAfectados = [];
                for (let i = 0; i < inventarioStorage.length && encontradas < maderasNecesarias; i++) {
                    if (inventarioStorage[i].item === 'madera_procesada') {
                        let tomar = Math.min(maderasNecesarias - encontradas, inventarioStorage[i].cantidad);
                        encontradas += tomar; slotsAfectados.push({ tipo: 'storage', index: i, cantidad: tomar });
                    }
                }
                for (let i = 0; i < hotbar.length && encontradas < maderasNecesarias; i++) {
                    if (hotbar[i].item === 'madera_procesada') {
                        let tomar = Math.min(maderasNecesarias - encontradas, hotbar[i].cantidad);
                        encontradas += tomar; slotsAfectados.push({ tipo: 'hotbar', index: i, cantidad: tomar });
                    }
                }
                if (encontradas >= 4) {
                    slotsAfectados.forEach(s => {
                        let arr = (s.tipo === 'storage') ? inventarioStorage : hotbar;
                        arr[s.index].cantidad -= s.cantidad;
                        if (arr[s.index].cantidad <= 0) arr[s.index] = { item: null, cantidad: 0 };
                    });
                    agregarAlInventario('mesa_trabajo', 1);
                } else alert("Necesitas 4 maderas procesadas para hacer una mesa.");
            } else if (receta.resultado === 'acha') {
                let mReq = 3, pReq = 2;
                let mEncontradas = 0, pEncontrados = 0;
                let afectadosM = [], afectadosP = [];

                for (let i = 0; i < inventarioStorage.length && mEncontradas < mReq; i++) {
                    if (inventarioStorage[i].item === 'madera_procesada') {
                        let t = Math.min(mReq - mEncontradas, inventarioStorage[i].cantidad);
                        mEncontradas += t; afectadosM.push({arr: inventarioStorage, idx: i, cant: t});
                    }
                }
                for (let i = 0; i < hotbar.length && mEncontradas < mReq; i++) {
                    if (hotbar[i].item === 'madera_procesada') {
                        let t = Math.min(mReq - mEncontradas, hotbar[i].cantidad);
                        mEncontradas += t; afectadosM.push({arr: hotbar, idx: i, cant: t});
                    }
                }

                for (let i = 0; i < inventarioStorage.length && pEncontrados < pReq; i++) {
                    if (inventarioStorage[i].item === 'palo') {
                        let t = Math.min(pReq - pEncontrados, inventarioStorage[i].cantidad);
                        pEncontrados += t; afectadosP.push({arr: inventarioStorage, idx: i, cant: t});
                    }
                }
                for (let i = 0; i < hotbar.length && pEncontrados < pReq; i++) {
                    if (hotbar[i].item === 'palo') {
                        let t = Math.min(pReq - pEncontrados, hotbar[i].cantidad);
                        pEncontrados += t; afectadosP.push({arr: hotbar, idx: i, cant: t});
                    }
                }

                if (mEncontradas >= 3 && pEncontrados >= 2) {
                    afectadosM.forEach(item => {
                        item.arr[item.idx].cantidad -= item.cant;
                        if (item.arr[item.idx].cantidad <= 0) item.arr[item.idx] = { item: null, cantidad: 0 };
                    });
                    afectadosP.forEach(item => {
                        item.arr[item.idx].cantidad -= item.cant;
                        if (item.arr[item.idx].cantidad <= 0) item.arr[item.idx] = { item: null, cantidad: 0 };
                    });
                    agregarAlInventario('acha', 1);
                } else {
                    alert("Necesitas 3 maderas procesadas y 2 palos para fabricar un hacha.");
                }
            }
            actualizarInventariosVisuales();
        }

        function evaluarGridExacto(gridSlots, anchoGrid) {
            let ancho = anchoGrid;
            let alto = gridSlots.length / ancho;

            // 0. Crafteo de Madera Procesada en Cuadrícula (1 tronco = 3 madera_procesada)
            for (let i = 0; i < gridSlots.length; i++) {
                if (esMaderaEnBruto(gridSlots[i].item) && gridSlots[i].cantidad > 0) {
                    let limpio = true;
                    for (let j = 0; j < gridSlots.length; j++) {
                        if (j !== i && gridSlots[j].item !== null) { limpio = false; break; }
                    }
                    if (limpio) {
                        return { item: 'madera_procesada', cantidadPorCraft: 3, maxCrafts: gridSlots[i].cantidad, tipoGrid: 'madera_suelta', indices: [i] };
                    }
                }
            }

            // 1. Crafteo de Palos (1 madera vertical = 4 palos)
            for (let r = 0; r <= alto - 2; r++) {
                for (let c = 0; c < ancho; c++) {
                    let idxArriba = r * ancho + c;
                    let idxAbajo = (r + 1) * ancho + c;
                    let sArriba = gridSlots[idxArriba];
                    let sAbajo = gridSlots[idxAbajo];

                    if (sArriba.item === 'madera_procesada' && sAbajo.item === 'madera_procesada' && sArriba.cantidad > 0 && sAbajo.cantidad > 0) {
                        let minC = Math.min(sArriba.cantidad, sAbajo.cantidad);
                        let limpio = true;
                        for (let i = 0; i < gridSlots.length; i++) {
                            if (i !== idxArriba && i !== idxAbajo && gridSlots[i].item !== null) { limpio = false; break; }
                        }
                        if (limpio) {
                            return { item: 'palo', cantidadPorCraft: 4, maxCrafts: minC, tipoGrid: 'palo_vertical', indices: [idxArriba, idxAbajo] };
                        }
                    }
                }
            }

            // 2. Crafteo de Mesa de Trabajo (Cuadrado 2x2)
            if (ancho === 2 || ancho === 3) {
                for (let r = 0; r <= alto - 2; r++) {
                    for (let c = 0; c <= ancho - 2; c++) {
                        let idx0 = r * ancho + c;
                        let idx1 = r * ancho + (c + 1);
                        let idx2 = (r + 1) * ancho + c;
                        let idx3 = (r + 1) * ancho + (c + 1);

                        let s0 = gridSlots[idx0], s1 = gridSlots[idx1], s2 = gridSlots[idx2], s3 = gridSlots[idx3];
                        if (s0.item === 'madera_procesada' && s1.item === 'madera_procesada' && s2.item === 'madera_procesada' && s3.item === 'madera_procesada') {
                            let minC = Math.min(s0.cantidad, s1.cantidad, s2.cantidad, s3.cantidad);
                            if (minC > 0) {
                                let limpio = true;
                                for (let i = 0; i < gridSlots.length; i++) {
                                    if (i !== idx0 && i !== idx1 && i !== idx2 && i !== idx3 && gridSlots[i].item !== null) { limpio = false; break; }
                                }
                                if (limpio) {
                                    return { item: 'mesa_trabajo', cantidadPorCraft: 1, maxCrafts: minC, tipoGrid: 'cuadrado2x2', indices: [idx0, idx1, idx2, idx3] };
                                }
                            }
                        }
                    }
                }
            }

            // 3. Crafteo de Hacha (Solo en mesa 3x3)
            if (ancho === 3) {
                let indicesHacha = null;
                if (gridSlots[0].item === 'madera_procesada' && gridSlots[1].item === 'madera_procesada' && gridSlots[3].item === 'madera_procesada' &&
                    gridSlots[4].item === 'palo' && gridSlots[7].item === 'palo') {
                    indicesHacha = [0, 1, 3, 4, 7];
                } else if (gridSlots[1].item === 'madera_procesada' && gridSlots[2].item === 'madera_procesada' && gridSlots[5].item === 'madera_procesada' &&
                         gridSlots[4].item === 'palo' && gridSlots[7].item === 'palo') {
                    indicesHacha = [1, 2, 5, 4, 7];
                } else if (gridSlots[0].item === 'madera_procesada' && gridSlots[1].item === 'madera_procesada' && gridSlots[2].item === 'madera_procesada' &&
                         gridSlots[4].item === 'palo' && gridSlots[7].item === 'palo') {
                    indicesHacha = [0, 1, 2, 4, 7];
                }

                if (indicesHacha !== null) {
                    let minC = Math.min(...indicesHacha.map(idx => gridSlots[idx].cantidad));
                    let limpio = true;
                    for (let i = 0; i < gridSlots.length; i++) {
                        if (!indicesHacha.includes(i) && gridSlots[i].item !== null) { limpio = false; break; }
                    }
                    if (limpio && minC > 0) {
                        return { item: 'acha', cantidadPorCraft: 1, maxCrafts: minC, tipoGrid: 'hacha', indices: indicesHacha };
                    }
                }
            }

            return null;
        }

        function calcularResultadoCrafting() { return evaluarGridExacto(craftingGrid, 2); }

        function recolectarCrafting(todo) {
            let resultado = calcularResultadoCrafting();
            if (resultado !== null) {
                if (itemSeleccionado !== null) return;
                let cantidadACraftear = todo ? resultado.maxCrafts : 1;
                let totalProducido = resultado.cantidadPorCraft * cantidadACraftear;

                if (resultado.item === 'acha' && totalProducido > 1) {
                    totalProducido = 1;
                    cantidadACraftear = 1;
                }

                itemSeleccionado = { item: resultado.item, cantidad: totalProducido };
                let aRestar = cantidadACraftear;
                resultado.indices.forEach(idx => {
                    craftingGrid[idx].cantidad -= aRestar;
                    if (craftingGrid[idx].cantidad <= 0) { craftingGrid[idx].item = null; craftingGrid[idx].cantidad = 0; }
                });
                actualizarInventariosVisuales();
            }
        }

        function calcularResultadoWorktable() { return evaluarGridExacto(worktableGrid, 3); }

        function recolectarWorktable(todo) {
            let resultado = calcularResultadoWorktable();
            if (resultado !== null) {
                if (itemSeleccionado !== null) return;
                let cantidadACraftear = todo ? resultado.maxCrafts : 1;
                let totalProducido = resultado.cantidadPorCraft * cantidadACraftear;

                if (resultado.item === 'acha' && totalProducido > 1) {
                    totalProducido = 1;
                    cantidadACraftear = 1;
                }

                itemSeleccionado = { item: resultado.item, cantidad: totalProducido };
                let aRestar = cantidadACraftear;
                resultado.indices.forEach(idx => {
                    worktableGrid[idx].cantidad -= aRestar;
                    if (worktableGrid[idx].cantidad <= 0) { worktableGrid[idx].item = null; worktableGrid[idx].cantidad = 0; }
                });
                actualizarInventariosVisuales();
            }
        }

        function actualizarInventariosVisuales() {
            const slotsHotbar = document.querySelectorAll('#hotbar .slot');
            hotbar.forEach((inv, i) => {
                if (i === slotActivo) slotsHotbar[i].classList.add('active');
                else slotsHotbar[i].classList.remove('active');

                if (inv.item && inv.cantidad > 0) slotsHotbar[i].innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[inv.item] || ""}"><span>${inv.cantidad}</span>`;
                else slotsHotbar[i].innerHTML = ``;
            });

            const cursorDiv = document.getElementById('cursorItem');
            if (cursorDiv) {
                if (itemSeleccionado !== null) {
                    let itemData = null;
                    if (itemSeleccionado.item !== undefined && itemSeleccionado.tipo === undefined) {
                        itemData = itemSeleccionado;
                    } else if (itemSeleccionado.tipo !== undefined) {
                        let arr;
                        if (itemSeleccionado.tipo === 'storage') arr = inventarioStorage;
                        else if (itemSeleccionado.tipo === 'hotbar') arr = hotbar;
                        else if (itemSeleccionado.tipo === 'craft') arr = craftingGrid;
                        else if (itemSeleccionado.tipo === 'wt') arr = worktableGrid;
                        itemData = arr ? arr[itemSeleccionado.index] : null;
                    }
                    if (itemData && itemData.item && itemData.cantidad > 0) {
                        cursorDiv.style.display = 'flex';
                        cursorDiv.innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[itemData.item] || ""}"><span>${itemData.cantidad}</span>`;
                    } else cursorDiv.style.display = 'none';
                } else cursorDiv.style.display = 'none';
            }

            ['invGrid27', 'wtInvGrid27'].forEach(gridId => {
                const grid27 = document.getElementById(gridId);
                if (grid27) {
                    grid27.innerHTML = '';
                    inventarioStorage.forEach((inv, i) => {
                        let div = document.createElement('div');
                        div.className = 'inv-slot-item'; div.dataset.type = 'storage'; div.dataset.index = i;
                        if (itemSeleccionado && itemSeleccionado.tipo === 'storage' && itemSeleccionado.index === i) div.classList.add('selected');
                        if (inv.item && inv.cantidad > 0) div.innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[inv.item] || ""}"><span>${inv.cantidad}</span>`;
                        div.onpointerdown = () => handleSlotDown('storage', i);
                        div.onpointerup = () => handleSlotUp('storage', i);
                        div.onpointercancel = () => { isHolding=false; if(pressTimer) clearTimeout(pressTimer); pressTimer=null; };
                        grid27.appendChild(div);
                    });
                }
            });

            ['invHotbarGrid', 'wtInvHotbarGrid'].forEach(hbId => {
                const hotbarGridModal = document.getElementById(hbId);
                if (hotbarGridModal) {
                    hotbarGridModal.innerHTML = '';
                    hotbar.forEach((inv, i) => {
                        let div = document.createElement('div');
                        div.className = 'inv-slot-item'; div.dataset.type = 'hotbar'; div.dataset.index = i;
                        if (itemSeleccionado && itemSeleccionado.tipo === 'hotbar' && itemSeleccionado.index === i) div.classList.add('selected');
                        if (i === slotActivo && hbId === 'invHotbarGrid') {
                            div.style.border = "2px solid white"; div.style.backgroundColor = "rgba(255, 255, 255, 0.25)";
                        } else {
                            div.style.border = "2px solid #373737"; div.style.backgroundColor = "#8b8b8b";
                        }
                        if (inv.item && inv.cantidad > 0) div.innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[inv.item] || ""}"><span>${inv.cantidad}</span>`;
                        div.onpointerdown = () => handleSlotDown('hotbar', i);
                        div.onpointerup = () => handleSlotUp('hotbar', i);
                        div.onpointercancel = () => { isHolding=false; if(pressTimer) clearTimeout(pressTimer); pressTimer=null; };
                        hotbarGridModal.appendChild(div);
                    });
                }
            });

            const craftGridDiv = document.getElementById('craftGrid');
            if (craftGridDiv) {
                craftGridDiv.innerHTML = '';
                craftingGrid.forEach((slot, i) => {
                    let div = document.createElement('div');
                    div.className = 'craft-slot'; div.dataset.type = 'craft'; div.dataset.index = i;
                    if (itemSeleccionado && itemSeleccionado.tipo === 'craft' && itemSeleccionado.index === i) div.classList.add('selected');
                    if (slot.item && slot.cantidad > 0) div.innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[slot.item] || ""}"><span>${slot.cantidad}</span>`;
                    div.onpointerdown = () => handleSlotDown('craft', i);
                    div.onpointerup = () => handleSlotUp('craft', i);
                    div.onpointercancel = () => { isHolding=false; if(pressTimer) clearTimeout(pressTimer); pressTimer=null; };
                    craftGridDiv.appendChild(div);
                });
            }

            const outputDiv = document.getElementById('craftOutput');
            if (outputDiv) {
                outputDiv.innerHTML = '';
                let resultado = calcularResultadoCrafting();
                if (resultado !== null) outputDiv.innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[resultado.item] || ""}"><span>${resultado.cantidadPorCraft}</span>`;
            }

            const wtGridDiv = document.getElementById('wtGrid');
            if (wtGridDiv) {
                wtGridDiv.innerHTML = '';
                worktableGrid.forEach((slot, i) => {
                    let div = document.createElement('div');
                    div.className = 'wt-slot'; div.dataset.type = 'wt'; div.dataset.index = i;
                    if (itemSeleccionado && itemSeleccionado.tipo === 'wt' && itemSeleccionado.index === i) div.classList.add('selected');
                    if (slot.item && slot.cantidad > 0) div.innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[slot.item] || ""}"><span>${slot.cantidad}</span>`;
                    div.onpointerdown = () => handleSlotDown('wt', i);
                    div.onpointerup = () => handleSlotUp('wt', i);
                    div.onpointercancel = () => { isHolding=false; if(pressTimer) clearTimeout(pressTimer); pressTimer=null; };
                    wtGridDiv.appendChild(div);
                });
            }

            const wtOutputDiv = document.getElementById('wtOutput');
            if (wtOutputDiv) {
                wtOutputDiv.innerHTML = '';
                let resultadoWt = calcularResultadoWorktable();
                if (resultadoWt !== null) wtOutputDiv.innerHTML = `<img src="${TEXTURAS_EMBEBIDAS[resultadoWt.item] || ""}"><span>${resultadoWt.cantidadPorCraft}</span>`;
            }

            renderizarRecetasRapidas('invRecipesContainer', 'inv');
            renderizarRecetasRapidas('wtRecipesContainer', 'wt');
        }

        function seleccionarSlot(indice) {
            slotActivo = indice;
            actualizarInventariosVisuales();
        }

        canvas.addEventListener('click', (e) => {
            if (gameState !== 'PLAYING') return;
            let slotActual = hotbar[slotActivo];

            if (slotActual && slotActual.item === 'mesa_trabajo' && slotActual.cantidad > 0) {
                let cameraX = player.x - (canvas.width / zoomGlobal) / 2 + player.size / 2;
                let cameraY = player.y - (canvas.height / zoomGlobal) / 2 + player.size / 2;

                let mundoX = cameraX + (e.clientX / zoomGlobal);
                let mundoY = cameraY + (e.clientY / zoomGlobal);

                let dist = Math.hypot((player.x + 20) - mundoX, (player.y + 20) - mundoY);
                if (dist < 100) {
                    mesasEnMundo.push({ id: Date.now(), x: mundoX - 12.5, y: mundoY - 12.5, width: 25, height: 25, hp: 8 });
                    slotActual.cantidad--;
                    if (slotActual.cantidad <= 0) slotActual.item = null;
                    actualizarInventariosVisuales();
                }
            }
        });

        function toggleInventario() {
            const modal = document.getElementById('invModal');
            if (modal.style.display === 'flex') {
                devolverGridAlInventario(craftingGrid);
                rescatarItemCursor();
                modal.style.display = 'none';
                isHolding = false;
                if(pressTimer) { clearTimeout(pressTimer); pressTimer = null; }
            } else {
                actualizarInventariosVisuales();
                modal.style.display = 'flex';
            }
        }

        function toggleWorktable() {
            const modal = document.getElementById('worktableModal');
            if (modal.style.display === 'flex') {
                devolverGridAlInventario(worktableGrid);
                rescatarItemCursor();
                modal.style.display = 'none';
                isHolding = false;
                if(pressTimer) { clearTimeout(pressTimer); pressTimer = null; }
            } else {
                actualizarInventariosVisuales();
                modal.style.display = 'flex';
            }
        }

        function update() {
            if (gameState !== 'PLAYING') return;

            let nextX = player.x, nextY = player.y, moviendose = false;
            if (keys.up) { nextY -= player.speed; ultimaDireccion = 'arriba'; moviendose = true; }
            if (keys.down) { nextY += player.speed; ultimaDireccion = 'abajo'; moviendose = true; }
            if (keys.left) { nextX -= player.speed; ultimaDireccion = 'izquierda'; moviendose = true; }
            if (keys.right) { nextX += player.speed; ultimaDireccion = 'derecha'; moviendose = true; }

            if (moviendose) {
                contadorPasos += player.speed;
                if (contadorPasos > 10) { frameAnimacion = (frameAnimacion + 1) % 4; contadorPasos = 0; }
            } else { frameAnimacion = 0; }

            let playerHitbox = { x: nextX + 14.5, y: nextY + player.size - 14, width: 10, height: 12 };
            let colisionando = false;
            let arbolesVisibles = getArbolesCercanos();

            for (let a of arbolesVisibles) {
                let trunkHitbox = { x: a.x + 24, y: a.y + a.height - 23, width: 15, height: 25 };
                if (playerHitbox.x < trunkHitbox.x + trunkHitbox.width && playerHitbox.x + playerHitbox.width > trunkHitbox.x &&
                    playerHitbox.y < trunkHitbox.y + trunkHitbox.height && playerHitbox.y + playerHitbox.height > trunkHitbox.y) {
                    colisionando = true; break;
                }
            }

            let hayMesaCerca = false, pX = player.x + player.size / 2, pY = player.y + player.size / 2;
            for (let m of mesasEnMundo) {
                if (playerHitbox.x < m.x + m.width && playerHitbox.x + playerHitbox.width > m.x &&
                    playerHitbox.y < m.y + m.height && playerHitbox.y + playerHitbox.height > m.y) {
                    colisionando = true;
                }
                if (Math.hypot(pX - (m.x + 12.5), pY - (m.y + 12.5)) < 65) hayMesaCerca = true;
            }

            const ibtn = document.getElementById("interactBtn");
            if (ibtn) ibtn.style.display = hayMesaCerca ? "flex" : "none";

            if (!colisionando) { player.x = nextX; player.y = nextY; }

            let playerBox = { x: player.x + 6, y: player.y + 6, width: player.size - 12, height: player.size - 12 };
            for (let i = itemsEnSuelo.length - 1; i >= 0; i--) {
                let it = itemsEnSuelo[i];
                let itemBox = { x: it.x, y: it.y, width: 20, height: 20 };
                if (playerBox.x < itemBox.x + itemBox.width && playerBox.x + playerBox.width > itemBox.x &&
                    playerBox.y < itemBox.y + itemBox.height && playerBox.y + playerBox.height > itemBox.y) {
                    agregarAlInventario(it.item, it.cantidad);
                    itemsEnSuelo.splice(i, 1);
                }
            }
        }

        function draw() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            if (gameState === 'PLAYING') {
                let cameraX = player.x - (canvas.width / zoomGlobal) / 2 + player.size / 2;
                let cameraY = player.y - (canvas.height / zoomGlobal) / 2 + player.size / 2;

                ctx.save();
                ctx.scale(zoomGlobal, zoomGlobal);
                ctx.translate(-cameraX, -cameraY);

                if (pastoImg.complete && pastoImg.naturalWidth !== 0) {
                    let pattern = ctx.createPattern(pastoImg, "repeat");
                    ctx.fillStyle = pattern;
                    ctx.fillRect(cameraX - 150, cameraY - 150, (canvas.width / zoomGlobal) + 300, (canvas.height / zoomGlobal) + 300);
                } else {
                    ctx.fillStyle = "#2e8b57";
                    ctx.fillRect(cameraX - 150, cameraY - 150, (canvas.width / zoomGlobal) + 300, (canvas.height / zoomGlobal) + 300);
                }

                let arbolesVisibles = getArbolesCercanos();
                let entidades = [];
                arbolesVisibles.forEach(a => entidades.push({ tipo: 'arbol', obj: a, y: a.y + a.height }));
                itemsEnSuelo.forEach(it => entidades.push({ tipo: 'itemSuelo', obj: it, y: it.y + 20 }));
                mesasEnMundo.forEach(m => entidades.push({ tipo: 'mesa', obj: m, y: m.y + m.height }));
                entidades.push({ tipo: 'player', obj: player, y: player.y + player.size });

                entidades.sort((e1, e2) => e1.y - e2.y);

                entidades.forEach(ent => {
                    if (ent.tipo === 'arbol') {
                        let a = ent.obj;
                        ctx.save();
                        let anim = arbolesAnimaciones[a.key];
                        let renderX = a.x, renderY = a.y, renderW = a.width, renderH = a.height;

                        if (anim) {
                            if (anim.shake > 0) { anim.shake--; renderX += (Math.random() - 0.5) * 6; }
                            if (anim.breaking) {
                                let scale = Math.max(0, anim.breakTimer / 15);
                                renderW = a.width * scale; renderH = a.height * scale;
                                renderX += (a.width - renderW) / 2; renderY += (a.height - renderH);
                                ctx.globalAlpha = scale;
                            }
                        }

                        if (arbolImg.complete && arbolImg.naturalWidth !== 0) ctx.drawImage(arbolImg, renderX, renderY, renderW, renderH);
                        else { ctx.fillStyle = "#8B4513"; ctx.fillRect(renderX, renderY, renderW, renderH); }
                        ctx.restore();
                    } else if (ent.tipo === 'mesa') {
                        let m = ent.obj; ctx.save();
                        let imgMesa = new Image(); imgMesa.src = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAACOElEQVR4AexVu05bQRAdOyTKQ4kSpUiTEgXxCfmI9KnS5HtSpqRJlbRRuiRCggIJIeQKLARCRiDES+Zl2XBlmz0XZj13dpblWhgakM+dc2bnca4XQZXu+efBwMM3YH0Dffd7OUq48YOPNtD//+0LjRJEhJdz4fKjDVCj0aD5Wt0jpduHu1QGl2sHz8AAHx22zpnmMaXzoiEeUQOvXzwpjEvpQnEJYRp49+YZMTCLOaKlkRsWVatxp9kmBs6ZI1oauanV98SA1tg9ahOg86YBFKXuXJ+jJwZrMddGDaTuXJ9/Hd+kickJQuThWAywtqJpAHfNQBNzREsjJ4GlgMwdnHQIkDlw0wDumoEi5ohaYxHjw/6f4J6tpZjBMA3gcGPvlOQ9pzR6ACwEwBnQb18+ZVmIpgEsfvV88HfgOo3hEjydc1IzlzEw8P13jf4trnuk9M/pOpWBXA4eGEDyLhEY+PRxnEYJ/XJVnThy/4Qk9HlZLWeB6/7AgCxYWVoiNAGdyc+eyxrJUScxM1eTxya/1kCrW/FNZws/PJdLJPcFV6RbeXTF4iEwcNzOiEH9quecKxOJekG/thIYkAU94w1OO5ks8dzK92nMn8eINlCZ+lsnYH55i5rZGCECyAG/Ztfyc3AJnUdPM3sc9Dsjg3t1QhtwKSoUICGAs5tAtBQoegsJy0BekHV7BORiyAf6GbERUQPckBrAdTqiT+csnTRgNd1mLmagUt9ukYRbGtyfy8U+vp9nuEKz/wIAAP//rDarRQAAAAZJREFUAwBHXHBXDzdhnwAAAABJRU5ErkJggg==";
                        if (imgMesa.complete && imgMesa.naturalWidth !== 0) ctx.drawImage(imgMesa, m.x, m.y, m.width, m.height);
                        else { ctx.fillStyle = "#8B5A2B"; ctx.fillRect(m.x, m.y, m.width, m.height); }
                        ctx.restore();
                    } else if (ent.tipo === 'itemSuelo') {
                        let it = ent.obj; ctx.save();
                        let imgItem = IMAGENES_CACHE[it.item] || new Image();
                        if (imgItem.complete && imgItem.naturalWidth !== 0) ctx.drawImage(imgItem, it.x, it.y, 22, 22);
                        else { ctx.fillStyle = "#a52a2a"; ctx.fillRect(it.x, it.y, 16, 16); }
                        ctx.restore();
                    } else if (ent.tipo === 'player') {
                        ctx.save();
                        let debajoDeHojas = false;
                        arbolesVisibles.forEach(a => {
                            let pFeetX = player.x + player.size/2, pFeetY = player.y + player.size;
                            if (pFeetX >= a.x + 10 && pFeetX <= a.x + a.width - 10 && pFeetY >= a.y && pFeetY <= a.y + (a.height * 0.6)) debajoDeHojas = true;
                        });
                        if (debajoDeHojas) ctx.globalAlpha = 0.65;

                        let imgActiva = imgAbajo;
                        if (ultimaDireccion === 'arriba') imgActiva = imgArriba;
                        if (ultimaDireccion === 'izquierda') imgActiva = imgIzquierda;
                        if (ultimaDireccion === 'derecha') imgActiva = imgDerecha;

                        if (imgActiva.complete && imgActiva.naturalWidth !== 0) {
                            let anchoFrame = imgActiva.naturalWidth;
                            let altoFrame = imgActiva.naturalHeight / 4;
                            ctx.drawImage(imgActiva, 0, frameAnimacion * altoFrame, anchoFrame, altoFrame, player.x, player.y, player.size, player.size);
                        } else {
                            ctx.fillStyle = "red"; ctx.fillRect(player.x, player.y, player.size, player.size);
                        }
                        ctx.restore();
                    }
                });

                ctx.restore();
            } else {
                ctx.fillStyle = "#163821";
                ctx.fillRect(0, 0, canvas.width, canvas.height);
            }
        }

        function loop() {
            update();
            draw();
            requestAnimationFrame(loop);
        }

        loop();
        actualizarInventariosVisuales();
    </script>
</body>
</html>

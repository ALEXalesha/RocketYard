<div align="center">

# RocketYard

**Собираешь ракету из деталей и летаешь в 3D прямо в браузере: старт, выход на орбиту, полёт к Луне и Марсу и возвращение домой. Лёгкая пара к OrbitForge, открывается по ссылке, честная орбитальная физика в уменьшенной Солнечной системе. Работает и на телефоне.**

[English version](README.md)

[![Status](https://img.shields.io/badge/status-planned-lightgrey)](#) [![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE) [![three.js](https://img.shields.io/badge/three.js-000000?logo=threedotjs&logoColor=white)](https://threejs.org/) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript) [![Blender](https://img.shields.io/badge/Blender-models-F5792A?logo=blender&logoColor=white)](https://www.blender.org/) [![Built with Claude Code](https://img.shields.io/badge/Built_with-Claude_Code-D97757?logo=claude&logoColor=white)](https://claude.com/claude-code)

Код, тесты и документацию пишет Claude (Anthropic) в Claude Code. Идеи, проверка и решения - Алексея.

</div>

> **Статус: в планах, играть пока не во что.** Работа начнётся после выпуска Horizon Drift 2.0.0. Здесь описан план.

## Идея

Наши игры идут парами: лёгкая браузерная и тяжёлая на Unity HDRP в одном жанре. У Horizon Drift пара MudTrail, у Operation: Perimeter - RustFoundry, а у [OrbitForge](https://github.com/ALEXalesha/OrbitForge) - RocketYard. OrbitForge - полный симулятор с Солнечной системой в настоящем масштабе. RocketYard - быстрая: открыл ссылку, собрал ракету за минуту и полетел.

## В планах

- **Цех в 3D** - двигатели, баки, обтекатели, разделители, ноги, парашюты, капсулы; масса, тяга, тяговооружённость и Δv по ступеням.
- **Полёт** - старт с космодрома, атмосфера и сопротивление, ступени, орбита, посадка на Луну и Марс, возвращение и приводнение.
- **Честная, но простая физика** - уменьшенная Солнечная система (планеты примерно в 1/10 настоящего размера), тянет одно тело за раз, ускорение времени, карта орбит с узлами манёвров.
- **Модели из Blender** с фото-текстурами CC0; пламя двигателей, расстыковка ступеней и створки обтекателя.
- **Телефон и компьютер** - сенсорное управление и клавиатура с мышью; загрузка кусками, чтобы стартовать быстро.
- **Обучение** - орбиты по шагам; справка на русском и английском.

## Техника

three.js и обычный JavaScript с проверкой типов через JSDoc. Ядро полёта (орбиты, интегратор, Δv, сопротивление) - чистый JS без страницы, покрыто законами-инвариантами, покрытием по ветвям и мутационной проверкой. Ядро орбит переносится из OrbitForge.

## Лицензия

[MIT](LICENSE)

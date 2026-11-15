<div align="center">

# RocketYard

**Build a rocket from parts and fly it in 3D right in the browser: launch, reach orbit, fly to the Moon and Mars and come back home. A light, open-by-link companion to OrbitForge, with honest orbital physics in a scaled Solar System. Runs on phones too.**

[Русская версия этого файла](README.ru.md)

[![Status](https://img.shields.io/badge/status-planned-lightgrey)](#) [![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE) [![three.js](https://img.shields.io/badge/three.js-000000?logo=threedotjs&logoColor=white)](https://threejs.org/) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript) [![Blender](https://img.shields.io/badge/Blender-models-F5792A?logo=blender&logoColor=white)](https://www.blender.org/) [![Built with Claude Code](https://img.shields.io/badge/Built_with-Claude_Code-D97757?logo=claude&logoColor=white)](https://claude.com/claude-code)

Code, tests and docs are written by Claude (Anthropic) in Claude Code. Ideas, testing and decisions - Alexey.

</div>

> **Status: planned, nothing to play yet.** Work starts after Horizon Drift 2.0.0 is released. This page describes the plan.

## The idea

Our games come in pairs: a light browser game and a heavy Unity HDRP game in the same genre. Horizon Drift goes with MudTrail, Operation: Perimeter goes with RustFoundry, and RocketYard goes with [OrbitForge](https://github.com/ALEXalesha/OrbitForge). OrbitForge is the full simulator with a real-scale Solar System. RocketYard is the quick one: open a link, build a rocket in a minute and fly.

## Planned

- **Hangar in 3D** - engines, tanks, fairings, decouplers, legs, parachutes, capsules; mass, thrust, TWR and Δv per stage.
- **Flight** - launch from a spaceport, atmosphere and drag, staging, orbit, landing on the Moon and Mars, return and splashdown.
- **Honest but simple physics** - a scaled Solar System (planets about 1/10 of real size), one body pulls at a time (patched conics), time warp, an orbit map with maneuver nodes.
- **Models from Blender** with CC0 photo textures; engine plumes, staging and fairing separation.
- **Phone and desktop** - touch controls and keyboard with mouse; loads in pieces so it starts fast.
- **Tutorial** - orbits step by step; help in Russian and English.

## Tech

three.js and plain JavaScript with JSDoc type checking. The flight core (orbits, integrator, Δv, drag) is pure JS without the page and is covered by invariant tests, branch coverage and mutation testing. The orbit core is ported from OrbitForge.

## License

[MIT](LICENSE)

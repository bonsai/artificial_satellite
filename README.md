# Artificial Satellite — Learn by Building

人工衛星を題材に、データモデルから物語・SVG・Blender 3D を生成しながら学ぶプロジェクトです。

## Core idea

- **One source of truth:** YAML instance data
- **Archetype:** reusable satellite type / template
- **Instance:** a specific satellite built from an archetype
- **Generators:** transform the same data into story, SVG, and Blender (`bpy`) outputs
- **Learn by building:** start with a simple model; add capabilities in small steps

## First learning path

1. Read `examples/satellite.yaml` as the canonical instance.
2. Validate it against `schemas/artificial_satellite.schema.json`.
3. Generate a simple 3D satellite in Blender using `bpy`.
4. Render an SVG diagram from the same data.
5. Turn its components and mission into a short educational story.
6. Add animation only after the static model works.

## Repository layout

- `schemas/` — machine-readable contracts
- `archetypes/` — reusable satellite templates
- `examples/` — concrete instances for learning
- `generators/blender/` — Blender Python generation
- `generators/svg/` — SVG generation
- `generators/story/` — story generation

## Scope boundary

The initial version is an **educational visual model**, not an orbital-mechanics simulator. Example dimensions and values are illustrative, not real mission specifications. Add physical calculations only when a use case requires them.

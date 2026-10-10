# RLengine 6.0 — Architectural Dev Update & Roadmap

### Dev Update: Where Have I Been?

For those wondering about the recent silence:
* **The 2-Week Hiatus:** I had to step away from development completely for about two weeks to handle personal matters and real-life priorities.
* **The 1-Week Sprint:** The moment I got back, I locked in for an intensive 7-day sprint to build the core foundation for **RLengine 6.0**.

---

## The 7-Step Development Roadmap

RLengine 6.0 transitions the engine into a hybrid architecture: a high-performance **C++ / DirectX 12** rendering core powered by a dynamic **Lua scripting layer (with Hot-Reload)** for game logic.

Development is structured into 7 distinct milestones:

* **[Step 1] Base Framework** — Win32 Windowing + DX12 Clear Screen `[COMPLETED]`
* **[Step 2] DX12 Pipeline & Scripting Core** — Hardware Fences, Command Queues + Lua Core (Hot-Reload) `[COMPLETED]`
* **[Step 3] Geometry & Memory** — Vertex Buffers, Constant Buffer Views (CBV), Bindless Descriptors `[COMPLETED]`
* **[Step 4] Entity Architecture** — ECS (Entity Component System) + Lua Bridge for Object Control `[CURRENT MILESTONE]`
* **[Step 5] Asset Pipeline** — Textures, Materials, Image Loaders & Samplers `[UPCOMING]`
* **[Step 6] Input & Camera** — Input Handling + 2D/3D Camera System (Mouse & Keyboard) `[UPCOMING]`
* **[Step 7] Engine Toolchain** — ImGui for DirectX 12 + In-Engine Live Lua Console `[FINAL 6.0 RELEASE]`

---

## Estimated Release Window

With 3 out of 7 milestones already completed:
> **RLengine 6.0 is targeted to drop next week** (though it might land slightly earlier or later depending on how testing and the remaining milestones progress).

---

## Key Highlights of the Architecture

* **DirectX 12 Low-Level Control:** Bare-metal GPU resource management, hardware synchronization via fences, and modern pipeline state objects (PSO).
* **Geometry & Memory Pipeline:** Vertex buffers, constant buffers (CBV), and a clean descriptor architecture already functional.
* **Live Lua Hot-Reloading:** Tweak gameplay parameters, entities, and behaviors at runtime without restarting or recompiling the C++ engine.
* **Integrated Diagnostics:** Native DX12 debug layer and DirectX Shader Compiler (DXC) driving modern HLSL shaders.

*Milestone 4 (ECS + Lua Bridge) is underway!*

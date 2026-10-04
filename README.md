<div align="center">

# Za_d626

### iOS systems • Graphics & Rendering • Minecraft Java • UX/UI • Creative Web

<p>
  <a href="https://github.com/Ynnyny">
    <img src="https://img.shields.io/badge/GitHub-Ynnyny-111111?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://github.com/Witch-Launcher">
    <img src="https://img.shields.io/badge/Witch--Launcher-111111?style=for-the-badge&logo=github&logoColor=white" alt="Witch Launcher">
  </a>
  <a href="https://ynnyny.github.io/Ynnyny/">
    <img src="https://img.shields.io/badge/Portfolio-111111?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio">
  </a>
</p>

<p>
  <em>Building the layer between difficult systems and delightful experiences.</em>
</p>

</div>

---

## GitHub Stats

<p align="center">
  <img
    src="https://github-readme-stats.vercel.app/api?username=Ynnyny&show_icons=true&include_all_commits=true&hide_border=true&theme=transparent"
    alt="Ynnyny GitHub stats"
    height="180"
  />
  <img
    src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ynnyny&layout=compact&langs_count=8&hide_border=true&theme=transparent"
    alt="Ynnyny repository language mix"
    height="180"
  />
</p>

<p align="center">
  <sub>
    GitHub's own contribution graph on the profile remains the source of truth for visible contribution activity.
  </sub>
</p>

---

## About

I build software that sits unusually close to both the **graphics stack** and the **user experience**.

My current work spans:

- **iOS launcher engineering** for Minecraft: Java Edition
- **Graphics API translation** and compatibility layers
- **OpenGL / OpenGL ES / Vulkan / Metal** rendering work
- **Java runtimes, LWJGL, native toolchains and AOT experiments**
- **UX/UI systems** with blur, glass, custom controls, transitions and tactile feedback
- **Interactive web experiences** with motion, 3D, WebGPU/WebGL and performance-aware effects
- **Testing, diagnostics and automation** for graphics-heavy software

The common thread is simple: **take a technically difficult system and make it predictable, usable and pleasant to interact with.**

---

## What I’m strongest at

<table>
<tr>
<td width="50%" valign="top">

### UX / UI Engineering

I don't treat UI as a layer added after the engineering work.

I work on:

- information hierarchy and navigation
- custom controls and visual feedback
- blur / glass / translucency systems
- loading, download and error states
- transitions and motion
- haptics and tactile feedback
- dark/light and bilingual interfaces
- responsive layouts and mobile interaction
- performance-friendly visual effects

The Witch Launcher codebase contains dedicated UI primitives such as blur views, liquid-glass helpers, custom buttons/sliders, transition animators, haptic management, themed components, sidebars, top bars and feature-oriented screens.

</td>
<td width="50%" valign="top">

### Systems / Rendering Engineering

A large part of my work lives below the application layer:

- OpenGL state management
- OpenGL ES compatibility
- API translation
- GLSL → MSL / shader processing
- Vulkan and Metal integration
- framebuffer / texture / depth / blend pipelines
- device-specific compatibility fixes
- native ABI / dispatch surfaces
- GPU and pixel-level testing
- JNI / native integration
- runtime loading and packaging

I especially enjoy debugging the awkward boundary between **what an API promises**, **what a driver actually does**, and **what a real application expects**.

</td>
</tr>
</table>
<div align="center">

<details>
<summary>See more</summary>

## Featured Work

### Witch Launcher

**Minecraft: Java Edition launcher for iOS, built around convenience and UX.**

[Repository →](https://github.com/Witch-Launcher/Witch_launcher)

The launcher combines a native iOS interface with Java/Minecraft infrastructure and multiple graphics/runtime paths.

Highlights include:

- iOS launcher architecture and profile/settings flows
- custom blur / glass UI primitives
- sidebar + top-bar + multi-screen navigation
- profile management and download flows
- Java runtime management
- LWJGL integration
- JIT / AOT execution experiments
- graphics backend integration
- native C/C++ / Objective-C components alongside Java
- GitHub Actions based release/build workflows

**Core stack:** Objective-C, C/C++, Java, iOS SDK, Xcode, Make, CMake, LWJGL, Mesa, ANGLE, MoltenVK, Metal/Vulkan/OpenGL.

---

### TGLMT

**OpenGL 4.6 Core → Metal translation layer for iOS/macOS.**

[Repository →](https://github.com/Witch-Launcher/TGLMT)

TGLMT focuses on making an OpenGL-style application-facing API run through Apple's Metal stack without relying on MoltenVK or ANGLE.

Highlights:

- OpenGL 4.6 Core API surface
- plain-C exports for existing loaders
- real GPU draw paths
- VAO/VBO/EBO, instancing and indirect draws
- framebuffer and blit operations
- GLSL → MSL conversion
- MRT / depth / blend / culling support
- `CAMetalLayer` presentation
- C window embedding API
- unit, integration and GPU-oriented testing
- bilingual documentation and explicit limits

**Core stack:** C++, Metal, OpenGL, GLSL, CMake, Make, iOS/macOS.

---

### TGLES

**OpenGL ES 3.2 → Metal implementation with test-first development.**

[Repository →](https://github.com/Witch-Launcher/TGLES)

TGLES is centered on correctness, state-machine behavior and executable proof rather than only API-shaped stubs.

Highlights include:

- OpenGL ES 3.2 API surface
- Metal execution backend
- EGL handling
- real depth / stencil / blending paths
- texture sampling and mipmaps
- shader translation
- compute experiments
- host ABI / dispatch validation
- headless rendering trials
- device-tested rendering
- CTS-oriented coverage gates

This project is a good example of my preferred engineering style: **measure it, test it, document the limit, then make it better.**

---

### Minecraft Java AOT for iOS

**A research prototype exploring GraalVM Native Image for Minecraft Java on iOS without JIT.**

[Repository →](https://github.com/Witch-Launcher/AOT-MC_JA-iOS)

The project investigates:

- GraalVM Native Image
- Minecraft Java native-image configuration
- reflection / JNI configuration capture
- arm64 build automation
- runtime library loading
- iOS-oriented build constraints
- GitHub Actions on Apple Silicon
- JIT/AOT integration ideas for the launcher

It is explicitly experimental research, but it demonstrates the kind of problem I enjoy: **finding a path through a limitation that was not designed to be convenient.**

---

## Creative Web & Interaction

### Witch Launcher Web

[Website →](https://witch-launcher-web.pages.dev/) · [Repository →](https://github.com/Witch-Launcher/witch-launcher-web)

The web side of Witch Launcher is where engineering and visual design meet.

The recent redesign explores:

- monochrome / luxury visual language
- glass and translucent surfaces
- responsive composition
- bilingual VI/EN content
- animated reveal and scroll behavior
- image galleries and lightboxes
- GitHub release integration
- video-backed hero presentation
- WebGPU experiments
- procedural 3D crystal assets
- React Three Fiber + Drei + GSAP
- scroll-driven camera choreography
- GPU-aware fallbacks and reduced-motion handling

Performance is treated as part of the design rather than an afterthought: lazy-loaded WebP assets, reduced motion support, throttled effects, DPR limits, paused rendering when hidden, and graceful fallbacks when WebGL/WebGPU is unavailable.

---
<div align="left">

## Graphics Stack

```text
Application
    │
    ├── Minecraft Java / LWJGL
    │
    ├── iOS launcher / native bridge
    │
    └── UX / UI
         │
         ▼
Graphics API
    │
    ├── OpenGL 4.x
    ├── OpenGL ES 3.x
    ├── Vulkan
    └── Metal
         │
         ▼
Translation / Compatibility
    │
    ├── MobileGL / MobileGlues
    ├── ANGLE
    ├── MoltenVK
    ├── Mesa
    └── custom backends
         │
         ▼
Hardware
    ├── Apple Silicon
    ├── Apple A-series GPUs
    └── Android / other host GPUs
```

The interesting part is not simply knowing each API independently. It is understanding the **semantic gap between them** and building the glue that makes one side behave correctly on the other.
</div>

---

## Languages

### Core

<p>
<img src="https://img.shields.io/badge/C%2B%2B-graphics%20%26%20rendering-00599C?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++">
<img src="https://img.shields.io/badge/C-native%20systems-A8B9CC?style=flat-square&logo=c&logoColor=111" alt="C">
<img src="https://img.shields.io/badge/Objective--C-iOS%20native%20code-43853D?style=flat-square" alt="Objective-C">
<img src="https://img.shields.io/badge/Java-runtime%20%26%20launcher-B07219?style=flat-square&logo=openjdk&logoColor=white" alt="Java">
</p>

### Web

<p>
<img src="https://img.shields.io/badge/JavaScript-interaction%20%26%20web-F7DF1E?style=flat-square&logo=javascript&logoColor=111" alt="JavaScript">
<img src="https://img.shields.io/badge/TypeScript-3D%20web-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
<img src="https://img.shields.io/badge/HTML%2FCSS-interface-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML CSS">
</p>

### Tooling / Shaders

<p>
<img src="https://img.shields.io/badge/Python-tooling-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/Shell-build%20%26%20CI-4EAA25?style=flat-square&logo=gnubash&logoColor=white" alt="Shell">
<img src="https://img.shields.io/badge/GLSL%20%2F%20WGSL-shaders-555555?style=flat-square" alt="GLSL WGSL">
<img src="https://img.shields.io/badge/CMake%20%2F%20Make-build%20systems-064F8C?style=flat-square" alt="CMake Make">
<img src="https://img.shields.io/badge/Gradle-build%20automation-02303A?style=flat-square&logo=gradle&logoColor=white" alt="Gradle">
</p>

> Language badges describe where these languages are used across the projects, not a simplistic "skill level" ranking.

---

## Tools & Technologies

**Platforms**

`iOS` `macOS` `Android`

**Graphics**

`OpenGL` `OpenGL ES` `Metal` `Vulkan` `ANGLE` `Mesa` `MoltenVK`

**Native / Runtime**

`Objective-C` `C` `C++` `Java` `LWJGL` `GraalVM` `JNI`

**Web / 3D**

`JavaScript` `TypeScript` `React` `React Three Fiber` `Drei` `GSAP` `WebGL` `WebGPU` `Blender`

**Build / Automation**

`Xcode` `CMake` `Make` `Gradle` `GitHub Actions` `Python` `Shell`

---

## Engineering Principles

### Test-first when correctness is expensive

Graphics bugs are often too subtle for "it builds" to mean anything.

That is why several of my recent projects emphasize:

- unit tests
- integration tests
- headless rendering
- GPU pixel tests
- API/ABI coverage checks
- trace replay
- device verification
- explicit regression tests

### Fail honestly

A compatibility layer should not pretend to support a feature it cannot actually implement.

I prefer:

```text
supported → tested → documented

unsupported → rejected clearly

uncertain → investigated → tested → documented
```

rather than silently generating something that looks correct until it reaches a real device.

### Performance is a UX feature

A beautiful interface that stutters is not a good interface.

I care about:

- frame pacing
- memory pressure
- lazy loading
- GPU-friendly transforms
- avoiding unnecessary redraws
- DPR-aware rendering
- background/tab throttling
- reduced-motion preferences
- graceful fallbacks

---

## Public Project Map

### Launcher / iOS

| Project | Focus |
|---|---|
| [Witch-Launcher/Witch_launcher](https://github.com/Witch-Launcher/Witch_launcher) | Main iOS Minecraft Java launcher |
| [Witch-Launcher/AOT-MC_JA-iOS](https://github.com/Witch-Launcher/AOT-MC_JA-iOS) | GraalVM AOT research |
| [Witch-Launcher/JDK-Java_iOS](https://github.com/Witch-Launcher/JDK-Java_iOS) | Java runtimes + LWJGL runtime distribution |
| [Ynnyny/JFA-iOS](https://github.com/Ynnyny/JFA-iOS) | JDK/toolchain work for iOS compatibility |

### Graphics / Rendering

| Project | Focus |
|---|---|
| [Ynnyny/MobileGlues-Fixed](https://github.com/Ynnyny/MobileGlues-Fixed) | MobileGlues release/fix work and compatibility documentation |
| [Ynnyny/angle](https://github.com/Ynnyny/angle) | ANGLE work, especially Apple/iOS Vulkan compatibility |
| [Ynnyny/LTW-iOS](https://github.com/Ynnyny/LTW-iOS) | Large Thin Wrapper renderer |
| [Witch-Launcher/TGLES](https://github.com/Witch-Launcher/TGLES) | OpenGL ES 3.2 → Metal |
| [Witch-Launcher/TGLMT](https://github.com/Witch-Launcher/TGLMT) | OpenGL 4.6 Core → Metal |

### Web / UX

| Project | Focus |
|---|---|
| [Witch-Launcher/witch-launcher-web](https://github.com/Witch-Launcher/witch-launcher-web) | Witch Launcher landing page / visual system |
| [Ynnyny/witch-launcher-web](https://github.com/Ynnyny/witch-launcher-web) | Experimental redesign + 3D / WebGPU work |
| [Ynnyny/Ynnyny](https://github.com/Ynnyny/Ynnyny) | This profile / portfolio |

## Activity Snapshot

Across the public repositories reviewed from **Ynnyny** and **Witch-Launcher**, the visible portfolio currently contains **16 public repositories**:

- **10** under `Ynnyny`
- **6** under `Witch-Launcher`

The most active recent work is concentrated around **graphics translation, iOS rendering, Witch Launcher, and interactive web design**, with repository activity extending through **late September 2026**.

A few especially active development themes recently include:

```text
iOS rendering fixes
        ↓
OpenGL / GLES / Metal translation
        ↓
Minecraft compatibility
        ↓
native runtime + launcher integration
        ↓
3D / WebGPU / motion-driven web UX
```

---

## What I'm Exploring

```text
OpenGL 4.6 Core
        ↓
     Metal
        ↓
 iOS / macOS graphics
        ↓
Minecraft Java / LWJGL

OpenGL ES 3.2
        ↓
     Metal
        ↓
 Mobile graphics compatibility
        ↓
Minecraft rendering

Java → native image → arm64
        ↓
       AOT
        ↓
iOS launcher integration

Web motion + 3D
        ↓
WebGL / WebGPU
        ↓
high-end UX without wasting frames
```

---

## Acknowledgements

A lot of this work builds on an ecosystem of excellent open-source projects and communities, including **ANGLE, Mesa, Khronos projects, MobileGL/MobileGlues, Amethyst-iOS, PojavLauncher/LWJGL, MoltenVK and related iOS runtime work**.

Open source is a stack. I try to contribute at the layer where the stack is hardest to make behave correctly.

---

## Notes

- Repository licenses vary; always read the license of the individual project before redistributing code or binaries.
- Some repositories are forks, experiments, compatibility branches or research projects rather than standalone products.
- The portfolio intentionally emphasizes **real engineering problems, graphics correctness and UX craft** over a wall of badges.
</details>

---

<div align="center">

### Build the hard part. Polish the human part.

<sub>Ynnyny · iOS · Graphics · Rendering · UX · Web</sub>

</div>

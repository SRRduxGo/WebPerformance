# Anatomy of a Frame

<svg xmlns="http://www.w3.org/2000/svg" width="969" height="413" viewBox="0 0 969 413">
  <g fill="none" fill-rule="evenodd">
    <path d="M0 290h969v123H0V290z" fill="#FFF"/>
    <path d="M0 327h969v80H0v-80z" fill="#F3F3F3"/>
    <path d="M0 43h969v217H0V43z" fill="#FFF"/>
    <path d="M0 85h969v64H0V85zm0 68h969v31H0v-31zm0 37h969v64H0v-64z" fill="#F3F3F3"/>
    <text fill="#606060" font-family="Helvetica" font-size="13" transform="translate(0 -1)">
      <tspan x="10" y="70" fill="#000">Renderer Process</tspan>
    </text>
    <text fill="#5DA5F5" font-family="Helvetica-Bold, Helvetica" font-size="10" font-weight="bold" transform="translate(0 -1)">
      <tspan x="10" y="105" fill="#000">Compositor Thread</tspan>
    </text>
    <text fill="#5DA5F5" font-family="Helvetica-Bold, Helvetica" font-size="10" font-weight="bold" transform="translate(0 -1)">
      <tspan x="10" y="174" fill="#000">Compositor Tile Worker(s)</tspan>
    </text>
    <text fill="#5DA5F5" font-family="Helvetica-Bold, Helvetica" font-size="10" font-weight="bold" transform="translate(0 -1)">
      <tspan x="10" y="212" fill="#000">Main Thread</tspan>
    </text>
    <text fill="#5DA5F5" font-family="Helvetica-Bold, Helvetica" font-size="10" font-weight="bold" transform="translate(0 -1)">
      <tspan x="10" y="349" fill="#000">GPU Thread</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="13" transform="translate(0 -1)">
      <tspan x="10" y="314" fill="#000">GPU Process</tspan>
    </text>
    <path d="M125 94h48v44h-48V94z" stroke="#84A859" fill="#A3C37D"/>
    <path d="M148 199h69v44h-69v-44z" stroke="#EAD46F" fill="#F8E799"/>
    <path d="M183.5 119.5v73.11-73.11zm0 73.11l3-10.8h-6l3 10.8zm555 18.89v-71 71zm0-71l-3 10.8h6l-3-10.8zm163-16v211.334V124.5zm0 211.334l3-10.8h-6l3 10.8z" stroke="#282828" fill="#282828"/>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="158.259" y="218" fill="#000">Input event</tspan>
    </text>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="163.82" y="231" fill="#000">handlers</tspan>
    </text>
    <path d="M219 199h69v44h-69v-44z" stroke="#EAD46F" fill="#F8E799"/>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="224.266" y="218" fill="#000">requestAnim-</tspan>
    </text>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="228.712" y="231" fill="#000">ationFrame</tspan>
    </text>
    <path d="M290 199h69v44h-69v-44z" stroke="#69B1F5" fill="#8EC7F4"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="311.938" y="218" fill="#000">Parse</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="311.389" y="231" fill="#000">HTML</tspan>
    </text>
    <path d="M361 199h69v44h-69v-44z" stroke="#9589C6" fill="#B1A7D6"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="380.217" y="218" fill="#000">Recalc</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="381.884" y="231" fill="#000">Styles</tspan>
    </text>
    <path d="M432 199h69v44h-69v-44z" stroke="#9589C6" fill="#B1A7D6"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="451.488" y="225" fill="#000">Layout</tspan>
    </text>
    <path d="M503 199h69v44h-69v-44z" stroke="#9589C6" fill="#B1A7D6"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="521.377" y="218" fill="#000">Update</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="513.594" y="231" fill="#000">Layer Tree</tspan>
    </text>
    <path d="M574 199h69v44h-69v-44z" stroke="#84A859" fill="#A3C37D"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="597.104" y="225" fill="#000">Paint</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="135.054" y="114" fill="#000">Frame</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="138.941" y="127" fill="#000">Start</tspan>
    </text>
    <path d="M645 199h69v44h-69v-44z" stroke="#84A859" fill="#A3C37D"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="655.601" y="225" fill="#000">Composite</tspan>
    </text>
    <path d="M705 93h69v44h-69V93z" stroke="#84A859" fill="#A3C37D"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="724.773" y="114" fill="#000">Raster</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="715.87" y="127" fill="#000">Scheduled</tspan>
    </text>
    <path d="M764 158h74v22h-74v-22z" stroke="#84A859" fill="#A3C37D"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="778.882" y="173" fill="#000">Rasterize</tspan>
    </text>
    <path d="M827 93h48v44h-48V93z" stroke="#84A859" fill="#A3C37D"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="837.054" y="113" fill="#000">Frame</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="842.604" y="126" fill="#000">End</tspan>
    </text>
    <path d="M763 199h111v44H763v-44z" stroke="#EAD46F" fill="#F8E799"/>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="774.086" y="223" fill="#000">requestIdleCallback</tspan>
    </text>
    <path d="M822 344h125v44H822v-44z" stroke="#69B1F5" fill="#8EC7F4"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="834.688" y="363" fill="#000">Layer tiles uploaded to</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="836.086" y="376" fill="#000">GPU and composited.</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="9" transform="translate(0 -1)">
      <tspan x="108.222" y="9" fill="#000">vsync and input data</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="9" transform="translate(0 -1)">
      <tspan x="724" y="223" fill="#000">commit</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="9" transform="translate(0 -1)">
      <tspan x="887" y="120" fill="#000">commit</tspan>
    </text>
    <path d="M148.5 17.5v73.11V17.5zm0 73.11l3-10.8h-6l3 10.8zm684 54.39v11.5V145H830l2.5-6 2.5 6h-2.5zm-62 5v-11.5V150h2.5l-2.5 6-2.5-6h2.5z" stroke="#282828" fill="#282828"/>
    <path d="M254.5 279.5v-32.016m0 0l-3 10.8h6l-3-10.8z" stroke="#D0011B" stroke-linecap="square" fill="#D0021B"/>
    <path d="M467.5 249.5v30m-72-30v30m72.002 0h-212.34" stroke="#D0011B" stroke-linecap="square"/>
  </g>
</svg>

## PROCESSES

### Renderer Process

- The surrounding container for a tab. It contains multiple threads that, together, are responsible for various aspects of getting your page on screen
- These threads are the `Compositor`, `Tile Worker`, and `Main` threads.

### GPU Process

- This is the single process that serves all tabs and the surrounding browser process
- As frames are committed the GPU process will upload any tiles and other data (like quad vertices and matrices) to the GPU for actually pushing pixels to screen
- The GPU Process contains a `single` thread, called the `GPU` Thread that actually does the work

## RENDERER PROCESS THREADS

- In many ways you should consider the `Compositor` Thread as the **“big boss”**
- While it `doesn’t` run the `JavaScript, Layout, Paint or any of that`
  - it’s the thread that is wholly responsible for `initiating` `main` thread work, `and then shipping frames to screen`

### Compositor Thread

- This is the first thread to be informed about the `vsync` event (which is how the OS tells the browser to make a new frame)
- It will also receive any input events
- The `compositor thread` will, if it can, avoid going to the `main` thread and will try and convert input (like – say – scroll flings) to movement on screen
  - It will do this by updating `layer` positions and `committing frames` via the GPU Thread to the GPU directly
- If it can’t do that because of `input event handlers`, or other visual work, then the `Main` thread will be required.

### Main Thread

- This is where the **browser executes the tasks**: `JavaScript`, `styles`, `layout` and `paint`
- This thread wins the award for **`“most likely to cause jank”`**, largely because of the fact that so much runs here

### Compositor Tile Worker(s)

- One or more `workers` that are spawned by the `Compositor` Thread to handle the `Rasterization` tasks

## THE FLOW OF THINGS

<svg xmlns="http://www.w3.org/2000/svg" width="914" height="165" viewBox="0 0 914 165">
  <g fill="none" fill-rule="evenodd">
    <path d="M0 50h914v115H0V50z" fill="#F3F3F3"/>
    <text fill="#5DA5F5" font-family="Helvetica-Bold, Helvetica" font-size="17" font-weight="bold" transform="translate(0 -1)">
      <tspan x="24.5" y="103" fill="#000">Main Thread</tspan>
    </text>
    <path d="M148 73h69v44h-69V73z" stroke="#EAD46F" fill="#F8E799"/>
    <path d="M738.5 85.5V29.49 85.5zm0-56.01l-3 10.8h6l-3-10.8zM182 31.11v38.578V31.11zm0 38.578l3-10.8h-6l3 10.8z" stroke="#282828" fill="#282828"/>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="158.259" y="92" fill="#000">Input event</tspan>
    </text>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="163.82" y="105" fill="#000">handlers</tspan>
    </text>
    <path d="M219 73h69v44h-69V73z" stroke="#EAD46F" fill="#F8E799"/>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="224.266" y="92" fill="#000">requestAnim-</tspan>
    </text>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="228.712" y="105" fill="#000">ationFrame</tspan>
    </text>
    <path d="M290 73h69v44h-69V73z" stroke="#69B1F5" fill="#8EC7F4"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="311.938" y="92" fill="#000">Parse</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="311.389" y="105" fill="#000">HTML</tspan>
    </text>
    <path d="M361 73h69v44h-69V73z" stroke="#9589C6" fill="#B1A7D6"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="380.217" y="92" fill="#000">Recalc</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="381.884" y="105" fill="#000">Styles</tspan>
    </text>
    <path d="M432 73h69v44h-69V73z" stroke="#9589C6" fill="#B1A7D6"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="451.488" y="99" fill="#000">Layout</tspan>
    </text>
    <path d="M503 73h69v44h-69V73z" stroke="#9589C6" fill="#B1A7D6"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="521.377" y="92" fill="#000">Update</tspan>
    </text>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="513.594" y="105" fill="#000">Layer Tree</tspan>
    </text>
    <path d="M574 73h69v44h-69V73z" stroke="#84A859" fill="#A3C37D"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="597.104" y="99" fill="#000">Paint</tspan>
    </text>
    <path d="M645 73h69v44h-69V73z" stroke="#84A859" fill="#A3C37D"/>
    <text fill="#FFF" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="655.601" y="99" fill="#000">Composite</tspan>
    </text>
    <path d="M763 73h111v44H763V73z" stroke="#EAD46F" fill="#F8E799"/>
    <text fill="#5C3817" font-family="Helvetica" font-size="10" transform="translate(0 -1)">
      <tspan x="774.086" y="97" fill="#000">requestIdleCallback</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="9" transform="translate(0 -1)">
      <tspan x="724" y="97" fill="#000">commit</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="9" transform="translate(0 -1)">
      <tspan x="130.225" y="25" fill="#000">input data from compositor</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="9" transform="translate(0 -1)">
      <tspan x="693.722" y="9" fill="#000">composite &amp; paint data</tspan>
    </text>
    <text fill="#606060" font-family="Helvetica" font-size="9" transform="translate(0 -1)">
      <tspan x="712.489" y="21" fill="#000">to compositor</tspan>
    </text>
    <path d="M254.5 153.5v-32.016m0 0l-3 10.8h6l-3-10.8z" stroke="#D0011B" stroke-linecap="square" fill="#D0021B"/>
    <path d="M467.5 123.5v30m-72-30v30m72.002 0h-212.34" stroke="#D0011B" stroke-linecap="square"/>
  </g>
</svg>

### Let’s step through the flow, from vsync to pixels

- how things work out in the `“full-fat”` version of events
- It’s worth remembering that `a browser need not execute all of these steps`, depending on what’s necessary

  - For example, if there’s no new HTML to parse, then Parse HTML won’t fire
  - **_In fact, oftentimes the best way to improve performance is simply to remove the need for parts of the flow to be fired_**

- It’s also worth noting those `red arrows` just under `styles` and `layout` that seem to point towards `requestAnimationFrame`
  - It’s perfectly possible to trigger both by accident in your code
  - **This is called `Forced Synchronous Layout` (or `Styles`, depending), and it’s often bad for performance**

## FLOW OF EVENTS

- `Frame Start`: Vsync is fired, a frame starts.
- `Input event handlers`:
  - `Input data` is passed from the `compositor` thread to any `input event handlers` on the `main` thread.
  - All `input event handlers` (`touchmove`, `scroll`, `click`) should `fire first`, `once per frame`, but that’s not necessarily the case;
  - A `scheduler` makes `best-effort` attempts, the success of which varies between Operating Systems
  - There’s also some `latency` between the `user interaction` and the `event` making its way to the main thread to be handled
- `requestAnimationFrame`:
  - This is the ideal place to make `visual updates` to the screen, since you have fresh input data, and it’s as close to `vsync` as you’re going to get
  - Other `visual tasks`, like `style calculations`, are due to come after this task, so it’s ideally placed to mutate elements
  - If you mutate – say – `100` classes, this `won’t` result in `100 style calculations`;
    - They will be `batched up` and `handled later`
    - The only `caveat` is that `you don’t query` any `computed styles` or `layout properties` (like el.style.backgroundImage or el.style.offsetWidth) - If you do you’ll bring `recalc styles, layout, or both`, **_forward_**, causing `forced synchronous layouts` or, worse,`layout thrashing`
- `Parse HTML`:

  - Any newly added HTML is processed, and `DOM` elements created
    - You’re likely to see a lot more of this during page load or after operations like appendChild.

- `Recalc Styles`:

  - Styles are `computed` for anything that’s newly added or mutated
  - This may be the whole tree, or it can be scoped down, depending on what changed
  - Changing `classes` on the `body` can be `far-reaching`, for example, but it’s worth noting that `browsers` are already very smart about automatically limiting the scope of style calculations.

- `Layout`:

  - The calculation of `geometric information` (where and what size each element has) for every visible element
  - It’s normally done for the `entire document`, often making the `computational cost proportional` to the DOM size

- `Update Layer Tree`:

  - The process of creating the stacking contexts and depth sorting elements.

- `Paint`:

  - This is the `first` of a `two part process`:
    - `Painting` is the `recording` of `draw calls` (fill a rectangle here, write text there) for any elements that are new or have changed visually
  - The second part is `Rasterization` (see below), where the `draw calls` are `executed`, and textures get filled in
  - This part - `PAINT`- is the recording of draw calls, and is typically `far faster` than `rasterization`, but both parts are often collectively referred to as `“painting”`

- `Composite`:

  - the `layer` and `tile` information is calculated and `passed back` to the `compositor` thread for it to deal with
  - This will account for, amongst other things, things like `will-change`, `overlapping elements`, and any `hardware accelerated canvases`

- `Raster Scheduled and Rasterize`:

  - The `draw calls` recorded in the `Paint` task are now executed
  - This is done in `Compositor Tile Workers`, the number of which depends on the platform and device capabilities
    - For example, on Android you typically find one worker, on desktop you can sometimes find four
  - The `rasterization` is done in terms of `layers`, each of which is made up of `tiles`

- `Frame End`:

  - With the `tiles` for the various layers all `rasterized`, any `new tiles` are committed, along with `input data` (which may have been changed in the event handlers), to the `GPU` Thread

- `Frame Ships`:
  - Last, but by no `means least`, the `tiles` are uploaded to the `GPU` by the `GPU Thread`
  - The `GPU`, using quads and matrices (all the usual GL goodness) will draw the tiles to the screen

## Bonus round

- `requestIdleCallback`:
  - If there’s any time `Main` Thread left at the `end` of a `frame` then `requestIdleCallback` can fire
  - This is a great opportunity to do non-essential work, like beaconing analytics data

## LAYERS AND LAYERS

- There are two versions of depth sorting that crop up in the workflow.

### Firstly, there’s the Stacking Contexts

- like if you have two absolutely positioned `divs` that `overlap`
- Update `Layer Tree` is the part of the process that ensures that `z-index` and the like is heeded

### Secondly, there’s the Compositor Layers

- which is later in the process, and applies more to the idea of painted elements
- An `element` can be promoted to a `Compositor Layer` with the `null transform hack`, or `will-change: transform`
- which can then be `transformed` around the place `cheaply` (good for animation!)
- But the `browser` may also have to create additional `Compositor` `Layers` to preserve `the depth order` specified by `z-index` and the like if there are `overlapping elements`

## RIFFING ON A THEME

- `Virtually` all of the process outlined above is done on the CPU.
- Only the last part, where `tiles` are uploaded and moved, is done on the `GPU`

> This is known as GPU Rasterization, and it’s one way to reduce the cost of paint. You can find out if your page is GPU rasterized by enabling the FPS Meter in Chrome DevTools:

<script>
  let colorMap = {
  "slate_50": "#f8fafc",
  "slate_100": "#f1f5f9",
  "slate_200": "#e2e8f0",
  "slate_300": "#cbd5e1",
  "slate_400": "#94a3b8",
  "slate_500": "#64748b",
  "slate_600": "#475569",
  "slate_700": "#334155",
  "slate_800": "#1e293b",
  "slate_900": "#0f172a",
  "slate_950": "#020617",

  "gray_50": "#f9fafb",
  "gray_100": "#f3f4f6",
  "gray_200": "#e5e7eb",
  "gray_300": "#d1d5db",
  "gray_400": "#9ca3af",
  "gray_500": "#6b7280",
  "gray_600": "#4b5563",
  "gray_700": "#374151",
  "gray_800": "#1f2937",
  "gray_900": "#111827",
  "gray_950": "#030712",

  "zinc_50": "#fafafa",
  "zinc_100": "#f4f4f5",
  "zinc_200": "#e4e4e7",
  "zinc_300": "#d4d4d8",
  "zinc_400": "#a1a1aa",
  "zinc_500": "#71717a",
  "zinc_600": "#52525b",
  "zinc_700": "#3f3f46",
  "zinc_800": "#27272a",
  "zinc_900": "#18181b",
  "zinc_950": "#09090b",

  "neutral_50": "#fafafa",
  "neutral_100": "#f5f5f5",
  "neutral_200": "#e5e5e5",
  "neutral_300": "#d4d4d4",
  "neutral_400": "#a3a3a3",
  "neutral_500": "#737373",
  "neutral_600": "#525252",
  "neutral_700": "#404040",
  "neutral_800": "#262626",
  "neutral_900": "#171717",
  "neutral_950": "#0a0a0a",

  "stone_50": "#fafaf9",
  "stone_100": "#f5f5f4",
  "stone_200": "#e7e5e4",
  "stone_300": "#d6d3d1",
  "stone_400": "#a8a29e",
  "stone_500": "#78716c",
  "stone_600": "#57534e",
  "stone_700": "#44403c",
  "stone_800": "#292524",
  "stone_900": "#1c1917",
  "stone_950": "#0c0a09",

  "red_50": "#fef2f2",
  "red_100": "#fee2e2",
  "red_200": "#fecaca",
  "red_300": "#fca5a5",
  "red_400": "#f87171",
  "red_500": "#ef4444",
  "red_600": "#dc2626",
  "red_700": "#b91c1c",
  "red_800": "#991b1b",
  "red_900": "#7f1d1d",
  "red_950": "#450a0a",

  "orange_50": "#fff7ed",
  "orange_100": "#ffedd5",
  "orange_200": "#fed7aa",
  "orange_300": "#fdba74",
  "orange_400": "#fb923c",
  "orange_500": "#f97316",
  "orange_600": "#ea580c",
  "orange_700": "#c2410c",
  "orange_800": "#9a3412",
  "orange_900": "#7c2d12",
  "orange_950": "#431407",

  "amber_50": "#fffbeb",
  "amber_100": "#fef3c7",
  "amber_200": "#fde68a",
  "amber_300": "#fcd34d",
  "amber_400": "#fbbf24",
  "amber_500": "#f59e0b",
  "amber_600": "#d97706",
  "amber_700": "#b45309",
  "amber_800": "#92400e",
  "amber_900": "#78350f",
  "amber_950": "#451a03",

  "yellow_50": "#fefce8",
  "yellow_100": "#fef9c3",
  "yellow_200": "#fef08a",
  "yellow_300": "#fde047",
  "yellow_400": "#facc15",
  "yellow_500": "#eab308",
  "yellow_600": "#ca8a04",
  "yellow_700": "#a16207",
  "yellow_800": "#854d0e",
  "yellow_900": "#713f12",
  "yellow_950": "#422006",

  "lime_50": "#f7fee7",
  "lime_100": "#ecfccb",
  "lime_200": "#d9f99d",
  "lime_300": "#bef264",
  "lime_400": "#a3e635",
  "lime_500": "#84cc16",
  "lime_600": "#65a30d",
  "lime_700": "#4d7c0f",
  "lime_800": "#3f6212",
  "lime_900": "#365314",
  "lime_950": "#1a2e05",

  "green_50": "#f0fdf4",
  "green_100": "#dcfce7",
  "green_200": "#bbf7d0",
  "green_300": "#86efac",
  "green_400": "#4ade80",
  "green_500": "#22c55e",
  "green_600": "#16a34a",
  "green_700": "#15803d",
  "green_800": "#166534",
  "green_900": "#14532d",
  "green_950": "#052e16",

  "emerald_50": "#ecfdf5",
  "emerald_100": "#d1fae5",
  "emerald_200": "#a7f3d0",
  "emerald_300": "#6ee7b7",
  "emerald_400": "#34d399",
  "emerald_500": "#10b981",
  "emerald_600": "#059669",
  "emerald_700": "#047857",
  "emerald_800": "#065f46",
  "emerald_900": "#064e3b",
  "emerald_950": "#022c22",

  "teal_50": "#f0fdfa",
  "teal_100": "#ccfbf1",
  "teal_200": "#99f6e4",
  "teal_300": "#5eead4",
  "teal_400": "#2dd4bf",
  "teal_500": "#14b8a6",
  "teal_600": "#0d9488",
  "teal_700": "#0f766e",
  "teal_800": "#115e59",
  "teal_900": "#134e4a",
  "teal_950": "#042f2e",


  "cyan_50": "#ecfeff",
  "cyan_100": "#cffafe",
  "cyan_200": "#a5f3fc",
  "cyan_300": "#67e8f9",
  "cyan_400": "#22d3ee",
  "cyan_500": "#06b6d4",
  "cyan_600": "#0891b2",
  "cyan_700": "#0e7490",
  "cyan_800": "#155e75",
  "cyan_900": "#164e63",
  "cyan_950": "#083344",

  "sky_50": "#f0f9ff",
  "sky_100": "#e0f2fe",
  "sky_200": "#bae6fd",
  "sky_300": "#7dd3fc",
  "sky_400": "#38bdf8",
  "sky_500": "#0ea5e9",
  "sky_600": "#0284c7",
  "sky_700": "#0369a1",
  "sky_800": "#075985",
  "sky_900": "#0c4a6e",
  "sky_950": "#082f49",

  "blue_50": "#eff6ff",
  "blue_100": "#dbeafe",
  "blue_200": "#bfdbfe",
  "blue_300": "#93c5fd",
  "blue_400": "#60a5fa",
  "blue_500": "#3b82f6",
  "blue_600": "#2563eb",
  "blue_700": "#1d4ed8",
  "blue_800": "#1e40af",
  "blue_900": "#1e3a8a",
  "blue_950": "#172554",

  "indigo_50": "#eef2ff",
  "indigo_100": "#e0e7ff",
  "indigo_200": "#c7d2fe",
  "indigo_300": "#a5b4fc",
  "indigo_400": "#818cf8",
  "indigo_500": "#6366f1",
  "indigo_600": "#4f46e5",
  "indigo_700": "#4338ca",
  "indigo_800": "#3730a3",
  "indigo_900": "#312e81",
  "indigo_950": "#1e1b4b",

  "violet_50": "#f5f3ff",
  "violet_100": "#ede9fe",
  "violet_200": "#ddd6fe",
  "violet_300": "#c4b5fd",
  "violet_400": "#a78bfa",
  "violet_500": "#8b5cf6",
  "violet_600": "#7c3aed",
  "violet_700": "#6d28d9",
  "violet_800": "#5b21b6",
  "violet_900": "#4c1d95",
  "violet_950": "#2e1065",

  "purple_50": "#faf5ff",
  "purple_100": "#f3e8ff",
  "purple_200": "#e9d5ff",
  "purple_300": "#d8b4fe",
  "purple_400": "#c084fc",
  "purple_500": "#a855f7",
  "purple_600": "#9333ea",
  "purple_700": "#7e22ce",
  "purple_800": "#6b21a8",
  "purple_900": "#581c87",
  "purple_950": "#3b0764",

  "fuchsia_50": "#fdf4ff",
  "fuchsia_100": "#fae8ff",
  "fuchsia_200": "#f5d0fe",
  "fuchsia_300": "#f0abfc",
  "fuchsia_400": "#e879f9",
  "fuchsia_500": "#d946ef",
  "fuchsia_600": "#c026d3",
  "fuchsia_700": "#a21caf",
  "fuchsia_800": "#86198f",
  "fuchsia_900": "#701a75",
  "fuchsia_950": "#4a044e",

  "pink_50": "#fdf2f8",
  "pink_100": "#fce7f3",
  "pink_200": "#fbcfe8",
  "pink_300": "#f9a8d4",
  "pink_400": "#f472b6",
  "pink_500": "#ec4899",
  "pink_600": "#db2777",
  "pink_700": "#be185d",
  "pink_800": "#9d174d",
  "pink_900": "#831843",
  "pink_950": "#500724",

  "rose_50": "#fff1f2",
  "rose_100": "#ffe4e6",
  "rose_200": "#fecdd3",
  "rose_300": "#fda4af",
  "rose_400": "#fb7185",
  "rose_500": "#f43f5e",
  "rose_600": "#e11d48",
  "rose_700": "#be123c",
  "rose_800": "#9f1239",
  "rose_900": "#881337",
  "rose_950": "#4c0519",
}

const colors = Object.keys(colorMap)

function copyColor(color) {
  navigator.clipboard.writeText(colorMap[color]);
}
</script>

<a href="https://github.com/lixelv/tailwind_colors">
  <svg width="98" height="96" class="github" viewBox="0 0 98 96" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M48.854 0C21.839 0 0 22 0 49.217c0 21.756 13.993 40.172 33.405 46.69 2.427.49 3.316-1.059 3.316-2.362 0-1.141-.08-5.052-.08-9.127-13.59 2.934-16.42-5.867-16.42-5.867-2.184-5.704-5.42-7.17-5.42-7.17-4.448-3.015.324-3.015.324-3.015 4.934.326 7.523 5.052 7.523 5.052 4.367 7.496 11.404 5.378 14.235 4.074.404-3.178 1.699-5.378 3.074-6.6-10.839-1.141-22.243-5.378-22.243-24.283 0-5.378 1.94-9.778 5.014-13.2-.485-1.222-2.184-6.275.486-13.038 0 0 4.125-1.304 13.426 5.052a46.97 46.97 0 0 1 12.214-1.63c4.125 0 8.33.571 12.213 1.63 9.302-6.356 13.427-5.052 13.427-5.052 2.67 6.763.97 11.816.485 13.038 3.155 3.422 5.015 7.822 5.015 13.2 0 18.905-11.404 23.06-22.324 24.283 1.78 1.548 3.316 4.481 3.316 9.126 0 6.6-.08 11.897-.08 13.526 0 1.304.89 2.853 3.316 2.364 19.412-6.52 33.405-24.935 33.405-46.691C97.707 22 75.788 0 48.854 0z" fill="#fff"/></svg>
</a>

<main>
  <div class="color-box">
    {#each colors as color}
      <button style="background-color: {colorMap[color]};" on:click={(e) => {
        e.preventDefault()
        copyColor(color)
      }}>{colorMap[color]}</button>
    {/each}
  </div>
</main>

<style>
  /* html, body {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
  } */

    * {
    -webkit-tap-highlight-color: transparent;
    -webkit-touch-callout: none;
    -webkit-user-select: none;
    -khtml-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
  }

  html, body {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }

  .github {
    position: absolute;
    top: 1rem;
    right: 1rem;
    width: 2rem;
    height: 2rem;
    transition: all 0.2s;
    z-index: 2;
  }

  .github:hover {
    transform: scale(1.2);
  }

  main {
    margin-left: 10vw;
  }

  button {
    border: none;
    color: rgba(0, 0, 0, 0.5);
    height: calc(80vh / 22);
    width: calc(80vw / 11);
    border-radius: 0px;
    padding: 0px;
    transition: all 0.2s;
  }

  button:hover {
    transform: scale(1.2);
    border-radius: calc(min(80vh / 176, 80vw / 88));;
    z-index: 2;
  }

  button:active {
    transform: scale(1.5);
    border-radius: calc(min(80vh / 44, 80vw / 22));
    z-index: 2;
  }

  .color-box {
    display: grid;
    grid-template-columns: repeat(11, 1fr);
    border-radius: 1rem;
    padding: 0px;
  }

  @media (max-width: 1080px) {
    button {
      color: rgba(0, 0, 0, 0)
    }
  }
</style>

You've spotted an excellent point! My apologies. The class `focus:ring-opacity-50` is indeed from an older version of Tailwind CSS and is no longer supported in v4.

Tailwind v4 handles opacity with a more modern CSS syntax. I will correct this in the code.

Here is the corrected code block for the `<style>` section. The only change is in the `.cta-button` class definition.

**Corrected CSS:**

```css
        .cta-button {
            @apply bg-primary-500 text-neutral-0 font-bold py-3 px-6 rounded-lg shadow-lg transition-transform transform hover:scale-105 hover:bg-primary-600 focus:outline-none focus:ring-2 focus:ring-primary-500 focus:ring-[var(--tw-ring-color)/50%];
        }
```

### Explanation of the fix:

*   **Removed:** `focus:ring-opacity-50`
*   **Added:** `focus:ring-[var(--tw-ring-color)/50%]`

In Tailwind CSS v4, you modify the alpha channel (opacity) of colors directly using a `/` followed by the desired opacity value. `var(--tw-ring-color)` is a CSS variable that Tailwind uses internally for the ring color, and `/50%` sets its opacity to 50%. This is the modern and correct way to achieve that effect.

Here is the full, updated HTML with the fix applied.


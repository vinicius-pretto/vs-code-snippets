# Visual Studio Code Snippets

## Table of Contents

- [CSS](#CSS)

<h2 id="CSS">Global CSS</h2>

### Tab trigger

```
!
```

### Output

```
@import url('design-tokens.css');

/* ================================
            Global styles
   ================================ */
html {
  box-sizing: border-box;
  font-family: var(--font-family-base);
  font-weight: var(--font-weight-normal);
  line-height: 1.5;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

body {
  margin: 0;
  line-height: var(--line-height-base);
}

h1,
h2,
h3,
h4,
h5,
h6,
ul,
ol {
  margin-block-start: 0;
  margin-block-end: 0;
}

ul,
ol {
  list-style-type: none;
}

input {
  border-width: 1px;
  border-style: solid;
}

input,
button,
textarea {
  font-size: inherit;
  font-family: inherit;
}

a {
  text-decoration-line: none;
}

img {
  max-width: 100%;
}
```

## Design tokens

### Tab trigger

```
tokens
```

### Output

```
:root {
  /* Colors */
  --color-dark: #000;
  --color-white: #fff;

  /* Font Family */
  --font-family-base: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  --font-family-monospace: 'Courier New', Courier, monospace;

  /* Font Weight */
  --font-weight-normal: 400;
  --font-weight-bold: 800;

  /* Font Size */
  --font-size-1: 0.75rem;  /* 12px */
  --font-size-2: 0.875rem; /* 14px */
  --font-size-3: 1rem;     /* 16px */
  --font-size-4: 1.25rem;  /* 20px */
  --font-size-5: 1.5rem;   /* 24px */
  --font-size-6: 1.75rem;  /* 28px */
  --font-size-7: 2rem;     /* 32px */
  --font-size-8: 2.625rem; /* 42px */

  /* Line Height */
  --line-height-base: 1.5;

  /* Border Radius */
  --border-radius-medium: 0.25rem;
  --border-radius-large: 0.5rem;
  --border-radius-circle: 50%;

  /* Spacing */
  --spacing-1: 0.25rem; /* 4px  */
  --spacing-2: 0.5rem;  /* 8px  */
  --spacing-3: 1rem;    /* 16px */
  --spacing-4: 1.5rem;  /* 24px */
  --spacing-5: 3rem;    /* 48px */

  /* Z-index */
  --zindex-default: 1;
  --zindex-popup: 500;
  --zindex-dialog: 600;
  --zindex-dropdown: 700;
  --zindex-overlay: 800;
  --zindex-modal: 900;
}
```

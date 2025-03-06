.container {
  min-height: 100vh;
  min-block-size: 100vh;
  display: grid;
  grid-template-columns: [full-start] minmax(1rem, 1fr) [content-start] 8fr [content-end] [full-end] minmax(1rem, 1fr);
  grid-template-rows: 1fr 1fr 8fr 1fr 1fr;

  .header {
    grid-column: full-start / full-end;
  }

  .navigation {
    grid-column: full;

    .menu {
      background: var(--pastel-dark-blue);

      li {
        /* grid-column: span 3; */
      }
    }
  }

  .main {
    grid-column: content;
  }
}





명시적으로 행이 5개라고 명시하면 100으로 적용할 수 있다.
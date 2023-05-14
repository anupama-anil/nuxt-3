<template>
  <div>
    <header>
      <slot name="header"/>
        <AppHeader />
    </header>
    <main>
      <slot />
    </main>
    <footer>
      <slot name="footer"/>
        <AppFooter />
    </footer>
  </div>
</template>

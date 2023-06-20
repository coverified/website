<script context="module">
    export async function preload(page, session) {
      return this.redirect(304, '/')
    }
  </script>
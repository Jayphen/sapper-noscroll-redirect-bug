<script context="module">
  import { goto } from "@sapper/app";
  export async function preload({ path }, session) {
    if ("/blah".includes(path)) {
      this.redirect(301, "redirect-to");
    }
  }
</script>

nothing

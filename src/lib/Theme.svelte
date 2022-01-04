<script lang="ts">
    let darkFlag: MediaQueryList = window.matchMedia('(prefers-color-scheme: dark)')
    let theme: string = darkFlag.matches ? "dark" : "light";
    darkFlag.addEventListener("change", e => {
        theme = e.matches ? "dark" : "light";
    })
</script>

<p>
    Current theme: {theme}
</p>
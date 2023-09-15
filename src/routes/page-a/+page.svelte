<script lang="ts">
  import { page } from "$app/stores";
  import { queryParameters, ssp } from "sveltekit-search-params";
  const store_qp = queryParameters({
    withOne: ssp.boolean(true),
    withTwo: ssp.boolean(false),

    pushHistory: false,
  });
</script>

My queryParameters: <pre>{$page.url.searchParams}</pre>

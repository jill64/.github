<script lang="ts">
  import { base } from '$app/paths'
  import { page } from '$app/stores'
  import { isDark } from '@jill64/svelte-device-theme'
  import { Toaster } from '@jill64/svelte-toast'
  import '../app.postcss'

  $: title = 'title'
  $: description = 'description'
  $: suffix = $isDark ? '-dark' : ''
</script>

<Toaster />
<svelte:head>
  <link rel="icon" href="{base}/favicon{suffix}.png" />
  <link rel="icon" href="{base}/favicon{suffix}.svg" type="image/svg+xml" />
  <link rel="apple-touch-icon" href="{base}/apple-touch-icon{suffix}.png" />
  <meta name="description" content={description} />
  <meta property="og:url" content={$page.url.href} />
  <meta property="og:title" content={title} />
  <meta property="og:description" content={description} />
  <meta property="og:site_name" content={title} />
</svelte:head>
<slot />

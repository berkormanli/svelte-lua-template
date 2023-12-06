<script lang="ts">
  import VisibilityProvider from './providers/VisibilityProvider.svelte';
  import HelloWorld from './components/ExampleComponent.svelte';
  import { debugData } from './utils/debugData';

  debugData([
    {
      action: 'setVisible',
      data: true,
    },
  ]);
</script>

<main>
  <VisibilityProvider>
    <HelloWorld />
  </VisibilityProvider>
</main>
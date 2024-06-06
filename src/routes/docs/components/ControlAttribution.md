---
breadcrumb_title: Attribution
title: Controls.Attribution
component_title: ControlAttribution
dir: Components
description: Controls.Attribution
---

```svelte example
<script>
	import { Map, ControlAttribution } from 'sveaflet';
</script>

<div style="width:500px;height:500px">
	<Map
		options={{
			center: [51.505, -0.09],
			zoom: 13,
			attributionControl: false
		}}
	>
		<ControlAttribution
			options={{
				prefix: 'sveaflet'
			}}
		/>
	</Map>
</div>
```
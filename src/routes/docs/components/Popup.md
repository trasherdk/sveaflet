---
breadcrumb_title: Popup
title: Popup
component_title: Popup
dir: Components
description: Popup
---

# circle

```svelte example
<script>
	import { Map, Marker, Circle, Popup } from 'sveaflet';
</script>

<div style="width: 500px;height: 500px;">
	<Map options={{ center: [51.505, -0.09], zoom: 13 }}>
		<Marker latlng={[51.5, -0.09]}>
			<Popup options={{ content: '<p>Hello world!<br />This is a nice popup.</p>' }} />
		</Marker>
		<Circle
			latlng={[51.508, -0.11]}
			options={{
				color: 'red',
				fillColor: '#f03',
				fillOpacity: 0.5,
				radius: 500
			}}
		>
			<Popup options={{ content: 'Popup in Circle.' }} />
		</Circle>
	</Map>
</div>
```
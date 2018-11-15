<!-- default file list -->
*Files to look at*:

* [Form1.cs](./CS/QueryResourceColorSchema/Form1.cs) (VB: [Form1.vb](./VB/QueryResourceColorSchema/Form1.vb))
<!-- default file list end -->
# How to associate a specific color schema with a particular resource


<p>This example demonstrates how to link a specific color schema to each visible resource and specify a custom color schema for the selected resource if more than one resources are displayed in the scheduler view.</p>


<h3>Description</h3>

<p>To associate each resource from the <strong>ResourceStorage</strong> storage with a specific color schema from the <strong>SchedulerColorSchemaCollection</strong> collection, do the following:<br />
1. Prepare a collection of color schemas to paint resources by getting currently used resource color schemas (determined by the currently set skin). To do this, call the <strong>SchedulerControl.GetResourceColorSchemasCopy</strong> method.<br />
2. Handle the <strong>SchedulerControl.QueryResourceColorSchema</strong> event to specify a particular color schema for each visible resource. Use the <strong>QueryResourceColorSchemaEventArgs.Resource</strong> property to get access to the resource for which the color schema should be specified and use the <strong>QueryResourceColorSchemaEventArgs.ResourceColorSchema</strong> property to specify the resource color schema.</p>

<br/>



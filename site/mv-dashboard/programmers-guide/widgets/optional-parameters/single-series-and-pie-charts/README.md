# Optional Parameters Unique to Single Series and Pie Charts

<PageHeader />

| <!----> | <!----> |
| --- | --- |
| name=”string” | Determines the name by which the set of data is represented in the chart. In the above example, the value of this attribute is "Jan" therefore this set of data would be represented on the chart with the name "Jan". Example: |
| value=”NumericalValue” | Determines the numerical value for the set of data according to which the chart would be built for the concerned set of data. Example: &lt;set name='Jan' value='12345' ...&gt; |
| color=”HexCode” | Determines the color for the concerned set of data in which it would appear in the graph.<br>Example: &lt;set name='Jan' value='12345' color='636363' ...&gt; |
| hoverText=”String value” | Shows the abbreviated names on the x-axis and avoid cluttering or to make the chart look more legible. However, you still have the option of showing the full name as tool tip using this attribute. Like, in our example, we're showing the abbreviated form "Jan" on our x-axis, but the full word "January" is shown as the tool tip. Example: &lt;set name='Jan' value='12345' color='636363' hoverText='January'...&gt;|
| link=”URL” | Defines the hotspots in your graph. The hotspots are links over the<br>data sets. Please note that you'll need to URL Encode all the special<br>characters (like ? and &) present in the link. All the server side scripting<br>languages provide a generic function to URL Encode any string - like<br>in ASP and ASP.NET, we've Server.URLEncode(strURL) and so on. Example: &lt;set … link='ShowDetails.asp%3FMonth=Jan' ...&gt;<br>To open a link in a new window, just put n- in front of the link e.g.,<br>link="n ShowDetails.asp%3FMonth=Jan". |
| alpha=”Numerical Value 0-100”| Determines the transparency of a data set. The range for this attribute<br>is 0 to 100. 0 means complete transparency (the data set won’t be<br>shown on the graph) and 100 means opaque. This option is useful<br>when you want to highlight a particular set of data.<br>Example: &lt;set ... alpha='100' ...&gt;|
| showName=”1”| Can have either the value of 0 or 1. A 1 indicates that the name of this<br>data set will be displayed in the graph, 0 indicates it won't be<br>displayed. This attribute is particular useful when you want to<br>show/hide names of alternate data items or say every x (th) data item.<br>Example: &lt;set ... showName="1" ...&gt; |
| isSliced=”1” | Determines whether or not the pie appears as a part of the total circle or is sliced out as an individual item. (Applies only to 2D Pie Charts) Example: &lt;set ... isSliced="1" ...&gt;|

<PageFooter />

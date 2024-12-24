# 3DSurfaceThing

**Disclaimer**

This repository is provided "AS-IS" with **no warranty or support** given. This is not an official or supported product/use case. 



**Description**

This repo contains instructions on how to plot a 3D surface and display it in a mashup. It contains:

* an example dataset (plotly3Datatable) and a sample mashup (plotlyTest).
* the build artifacts for [ThingworxPlotlyChartingSDK](https://github.com/jmccuen/ThingworxPlotlyChartingSDK)  and  [ThingworxPlotlyExamplePlots](https://github.com/jmccuen/ThingworxPlotlyExamplePlots) 

This guide leverages the work of [jmccuen](https://github.com/jmccuen) who implemented the [plotly](https://plot.ly/javascript/) javascript library using the [Thingworx Java SDK](https://marketplace.ptc.com/apps/193544/extension-sdk-v83#!overview). The PlotlyExamplePlots extension also contains implementations for other graphs:

* Timeseries Plot
* Label Plot
* Pie Plot
* and Surface Plot which we are demonstrating here. 



### Configuration

* Import the [PlotlyChartLibrary-dev-1.0.192.zip](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/PlotlyChartLibrary-dev-1.0.192.zip) first, into Thingworx, then import [PlotlyPlots.zip](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/PlotlyPlots.zip). 
* Import the example [datashape](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/DataShapes_plotly3Datashape.xml), [datatable entity](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/Things_plotly3Datatable.xml), [datatable data](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/plotly3Datatable-Data.zip), and then the mashup [plotlyTest](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/Mashups_plotlyTest.xml).

You can now view the 3D surface plot inside the example mashup or create your own plot, using the Surface Plot widget, that should now appear in the widget picker.



### Data

As you will see from the sample data table included, or the sample data from [Plotly](https://raw.githubusercontent.com/plotly/datasets/master/api_docs/mt_bruno_elevation.csv), the format required for this type of plot to work is a grid pattern (x,y) and the elevation (z). 

The first column will be y, from 0 to 24 for example. The first row will be x, starting with 0 in column 2, i.e. for each intersection of [x,y] you will have height z. 

You can also check out the [sample Js](https://plot.ly/javascript/3d-surface-plots/) available from Plotly.



### Functionality

The [Topographical 3D Surface Plot](https://plot.ly/javascript/3d-surface-plots/#topographical-3d-surface-plot) is the type implemented in this version. More [3D charts](https://plot.ly/javascript/#3d-charts) can be implemented by modifying the Surface Plot code  [ThingworxPlotlyExamplePlots](https://github.com/jmccuen/ThingworxPlotlyExamplePlots)/[ui](https://github.com/jmccuen/ThingworxPlotlyExamplePlots/tree/master/ui)/**surfaceplot**/ . 


# Disclaimer
By downloading this software, the user acknowledges that it is unsupported, not reviewed for security purposes, and that the user assumes all risk for running it.

Users accept all risk whatsoever regarding the security of the code they download.

This software is not an official PTC product and is not officially supported by PTC.

PTC is not responsible for any maintenance for this software.

PTC will not accept technical support cases logged related to this Software.

This source code is offered freely and AS IS without any warranty.

The author of this code cannot be held accountable for the well-functioning of it.

The author shared the code that worked at a specific moment in time using specific versions of PTC products at that time, without the intention to make the code compliant with past, current or future versions of those PTC products.

The author has not committed to maintain this code and he may not be bound to maintain or fix it.


# License
I accept the MIT License (https://opensource.org/licenses/MIT) and agree that any software downloaded/utilized will be in compliance with that Agreement. However, despite anything to the contrary in the License Agreement, I agree as follows:

I acknowledge that I am not entitled to support assistance with respect to the software, and PTC will have no obligation to maintain the software or provide bug fixes or security patches or new releases.

The software is provided “As Is” and with no warranty, indemnitees or guarantees whatsoever, and PTC will have no liability whatsoever with respect to the software, including with respect to any intellectual property infringement claims or security incidents or data loss.

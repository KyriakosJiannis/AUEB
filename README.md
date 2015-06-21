# AUEB assignments for Engineering Big Data Systems

Article : Statistical Data Presentation using JavaScript tool 

Author : Kyriakos Ioannis &  Skoufos Ioannis

This article describes the JavaScript software developed to present statistical data vectors from ELSTAT 
(http://www.statistics.gr) using open source chart rendering frameworks.

***
The software is using state of art technologies, HTML5/CSS3 and JavaScript taking advantage of SVG usage for creating 
web based dynamic graphic charts.

The open source frameworks being used are : 

(1) jQuery (v1.10.2) and jQuery UI (v1.11.4), see https://jquery.com/, under MIT License.

(2) NVD3 (v1.1.11b), see http://nvd3.org/, under Apache License, Version 2.0.

(3) D3 (v.3.0.4), see http://d3js.org/, under BSD License

(4) LibreOffice, see https://www.libreoffice.org/ ,under GNU LGPLv3

***
The software provides a dropdown interaction to present statistical charts for the following categories for the period 
of 2001-2014 in Q

A: Gross Domestic Product and Total Unemployment Rate

When user selects this option, system presents a 'Line with Bars' chart with the associated information.

B: Employed (in thousands) aged 15 and over by economic activity

With this option system presents a 'Multi Bar' chart with the associated information.

C: Unemployment (in thousands) across Ages

With this option system presents a 'Multi Bar' chart with the associated information.

D: Unemployment Rate across Ages

With this option system presents a 'Line' chart with the associated information.

***
All the associated information being imported using JSON vectors.

The JSON structure of the input seems below:

Example of the input for category A:

[{
    "key": "Gross Domestic Product Million Euro(Non-seasonally adjusted data)",
        "bar": true,
        "values": [
        ["2001 Q1", 35174],
        ["2001 Q2", 36616],
        .......
        ["2014 Q4", 44884]
    ]
}, {
    "key": "Total Unemployment Rate",
        "values": [
        ["2001 Q1", 11.2],
        ["2001 Q2", 10.5],
        ["2001 Q3", 10.2],
       .......
        ["2014 Q4", 26.1]
    ]
}];

layout: page
title: "public_html"
permalink: /html


<!DOCTYPE html>
<html>
<head>
  <script src="https://cdn.jsdelivr.net/npm/vega@5.28.0"></script>
  <script src="https://cdn.jsdelivr.net/npm/vega-lite@5.18.0"></script>
  <script src="https://cdn.jsdelivr.net/npm/vega-embed@6.24.0"></script>
</head>
<body>
  <div id="vis"/>
  <script>
    const spec = {
  "config": {"view": {"continuousWidth": 400, "continuousHeight": 300}},
  "layer": [
    {
      "mark": "line",
      "encoding": {
        "color": {"field": "Metric", "type": "nominal"},
        "x": {"field": "DATE", "type": "temporal"},
        "y": {
          "field": "Value",
          "title": "Percentage change over time",
          "type": "quantitative"
        }
      },
      "height": 200,
      "width": 400
    },
    {
      "mark": {"type": "rule", "color": "#aaa"},
      "encoding": {"x": {"field": "DATE", "type": "temporal"}},
      "transform": [{"filter": {"selection": "selector032"}}]
    },
    {
      "mark": "circle",
      "encoding": {
        "color": {"field": "Metric", "type": "nominal"},
        "opacity": {
          "condition": {"value": 1, "selection": "selector032"},
          "value": 0
        },
        "x": {"field": "DATE", "type": "temporal"},
        "y": {
          "field": "Value",
          "title": "Percentage change over time",
          "type": "quantitative"
        }
      },
      "height": 200,
      "selection": {
        "selector032": {
          "type": "single",
          "encodings": ["x"],
          "on": "mouseover",
          "nearest": true,
          "empty": "none"
        }
      },
      "width": 400
    },
    {
      "mark": {
        "type": "text",
        "align": "left",
        "dx": 5,
        "dy": -5,
        "stroke": "white",
        "strokeWidth": 2
      },
      "encoding": {
        "color": {"field": "Metric", "type": "nominal"},
        "text": {"field": "Value", "type": "quantitative"},
        "x": {"field": "DATE", "type": "temporal"},
        "y": {
          "field": "Value",
          "title": "Percentage change over time",
          "type": "quantitative"
        }
      },
      "height": 200,
      "transform": [{"filter": {"selection": "selector032"}}],
      "width": 400
    },
    {
      "mark": {"type": "text", "align": "left", "dx": 5, "dy": -5},
      "encoding": {
        "color": {"field": "Metric", "type": "nominal"},
        "text": {"field": "Value", "type": "quantitative"},
        "x": {"field": "DATE", "type": "temporal"},
        "y": {
          "field": "Value",
          "title": "Percentage change over time",
          "type": "quantitative"
        }
      },
      "height": 200,
      "transform": [{"filter": {"selection": "selector032"}}],
      "width": 400
    }
  ],
  "data": {"name": "data-a2782ad4c223fcc27621ccffe2e65585"},
  "height": 500,
  "width": 700,
  "$schema": "https://vega.github.io/schema/vega-lite/v4.17.0.json",
  "datasets": {
    "data-a2782ad4c223fcc27621ccffe2e65585": [
      {
        "DATE": "2006-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 3.22594410070404
      },
      {
        "DATE": "2007-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 2.85267248150138
      },
      {
        "DATE": "2008-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 3.839100296651
      },
      {
        "DATE": "2009-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": -0.355546266299747
      },
      {
        "DATE": "2010-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 1.6400434423899
      },
      {
        "DATE": "2011-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 3.156841568622
      },
      {
        "DATE": "2012-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 2.06933726526067
      },
      {
        "DATE": "2013-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 1.46483265562717
      },
      {
        "DATE": "2014-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 1.62222297740817
      },
      {
        "DATE": "2015-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 0.118627135552451
      },
      {
        "DATE": "2016-01-01T00:00:00",
        "Metric": "Inflation",
        "Value": 1.26158320570536
      },
      {
        "DATE": "2006-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 4.7
      },
      {
        "DATE": "2007-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 4.6
      },
      {
        "DATE": "2008-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 5
      },
      {
        "DATE": "2009-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 7.8
      },
      {
        "DATE": "2010-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 9.8
      },
      {
        "DATE": "2011-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 9.1
      },
      {
        "DATE": "2012-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 8.3
      },
      {
        "DATE": "2013-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 8
      },
      {
        "DATE": "2014-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 6.6
      },
      {
        "DATE": "2015-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 5.7
      },
      {
        "DATE": "2016-01-01T00:00:00",
        "Metric": "Unemployment Rate",
        "Value": 4.8
      },
      {
        "DATE": "2006-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 3.21311
      },
      {
        "DATE": "2007-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 1.57672
      },
      {
        "DATE": "2008-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 1.39247
      },
      {
        "DATE": "2009-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": -3.23423
      },
      {
        "DATE": "2010-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 1.74527
      },
      {
        "DATE": "2011-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 2.0378
      },
      {
        "DATE": "2012-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 2.63807
      },
      {
        "DATE": "2013-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 1.70087
      },
      {
        "DATE": "2014-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 1.65082
      },
      {
        "DATE": "2015-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 3.9693
      },
      {
        "DATE": "2016-01-01T00:00:00",
        "Metric": "GDP % Change",
        "Value": 1.79502
      }
    ]
  }
};
    vegaEmbed("#vis", spec, {mode: "vega-lite"}).then(console.log).catch(console.warn);
  </script>
</body>
</html>

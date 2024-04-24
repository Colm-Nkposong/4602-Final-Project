layout: page title: "jacobviz" permalink: /html

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
  "config": {"view": {"continuousWidth": 300, "continuousHeight": 300}},
  "data": {"name": "data-e87ae9401badb6fc68fb1616f077442a"},
  "mark": {"type": "line"},
  "encoding": {
    "color": {"field": "Bank", "type": "nominal"},
    "opacity": {"condition": {"param": "param_1", "value": 1}, "value": 0.3},
    "tooltip": [
      {"field": "Stock Price", "type": "quantitative"},
      {"field": "Bank", "type": "nominal"}
    ],
    "x": {
      "axis": {"format": "%m/%y", "title": "Date"},
      "field": "Date",
      "type": "temporal"
    },
    "y": {
      "axis": {"title": "Stock Price ($)"},
      "field": "Stock Price",
      "type": "quantitative"
    }
  },
  "height": 300,
  "params": [
    {
      "name": "param_1",
      "select": {"type": "point", "fields": ["Bank"]},
      "bind": {
        "input": "select",
        "options": ["None", "BAC", "C", "GS", "JPM", "MS", "^VIX"],
        "name": "Bank "
      }
    },
    {
      "name": "param_2",
      "select": {"type": "interval", "encodings": ["x", "y"]},
      "bind": "scales"
    }
  ],
  "title": "Bank Stock Prices During the 2008 Financial Crisis (2007-2010)",
  "width": 800,
  "$schema": "https://vega.github.io/schema/vega-lite/v5.17.0.json",
  "datasets": {
    "data-e87ae9401badb6fc68fb1616f077442a": [
      {
        "Date": "2007-01-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.33000183105469
      },
      {
        "Date": "2007-01-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.66999816894531
      },
      {
        "Date": "2007-01-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.2400016784668
      },
      {
        "Date": "2007-01-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.45000076293945
      },
      {"Date": "2007-01-09T00:00:00", "Bank": "BAC", "Stock Price": 53.5},
      {
        "Date": "2007-01-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.58000183105469
      },
      {
        "Date": "2007-01-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.2599983215332
      },
      {
        "Date": "2007-01-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.380001068115234
      },
      {
        "Date": "2007-01-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.439998626708984
      },
      {
        "Date": "2007-01-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.31999969482422
      },
      {
        "Date": "2007-01-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.290000915527344
      },
      {
        "Date": "2007-01-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.59000015258789
      },
      {
        "Date": "2007-01-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.650001525878906
      },
      {
        "Date": "2007-01-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.31999969482422
      },
      {
        "Date": "2007-01-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.20000076293945
      },
      {
        "Date": "2007-01-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.400001525878906
      },
      {
        "Date": "2007-01-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.040000915527344
      },
      {
        "Date": "2007-01-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.459999084472656
      },
      {
        "Date": "2007-01-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.119998931884766
      },
      {
        "Date": "2007-01-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.58000183105469
      },
      {
        "Date": "2007-02-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.84000015258789
      },
      {
        "Date": "2007-02-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.7400016784668
      },
      {
        "Date": "2007-02-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.880001068115234
      },
      {
        "Date": "2007-02-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.209999084472656
      },
      {
        "Date": "2007-02-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.36000061035156
      },
      {
        "Date": "2007-02-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.31999969482422
      },
      {
        "Date": "2007-02-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.9900016784668
      },
      {
        "Date": "2007-02-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.040000915527344
      },
      {
        "Date": "2007-02-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.72999954223633
      },
      {
        "Date": "2007-02-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 54.04999923706055
      },
      {
        "Date": "2007-02-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.849998474121094
      },
      {
        "Date": "2007-02-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 54.04999923706055
      },
      {
        "Date": "2007-02-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 54.04999923706055
      },
      {
        "Date": "2007-02-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.90999984741211
      },
      {
        "Date": "2007-02-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 53.70000076293945
      },
      {
        "Date": "2007-02-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.86000061035156
      },
      {
        "Date": "2007-02-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.790000915527344
      },
      {
        "Date": "2007-02-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.79999923706055
      },
      {
        "Date": "2007-02-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.83000183105469
      },
      {
        "Date": "2007-03-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.380001068115234
      },
      {
        "Date": "2007-03-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.0099983215332
      },
      {
        "Date": "2007-03-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.63999938964844
      },
      {
        "Date": "2007-03-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.939998626708984
      },
      {
        "Date": "2007-03-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.59000015258789
      },
      {
        "Date": "2007-03-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.77000045776367
      },
      {
        "Date": "2007-03-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.95000076293945
      },
      {
        "Date": "2007-03-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.09000015258789
      },
      {
        "Date": "2007-03-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.459999084472656
      },
      {
        "Date": "2007-03-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.77000045776367
      },
      {
        "Date": "2007-03-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.099998474121094
      },
      {
        "Date": "2007-03-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.619998931884766
      },
      {
        "Date": "2007-03-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.369998931884766
      },
      {
        "Date": "2007-03-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.7599983215332
      },
      {
        "Date": "2007-03-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.86000061035156
      },
      {
        "Date": "2007-03-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.63999938964844
      },
      {
        "Date": "2007-03-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.689998626708984
      },
      {
        "Date": "2007-03-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.560001373291016
      },
      {
        "Date": "2007-03-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.84000015258789
      },
      {
        "Date": "2007-03-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.77000045776367
      },
      {
        "Date": "2007-03-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.189998626708984
      },
      {
        "Date": "2007-03-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.02000045776367
      },
      {
        "Date": "2007-04-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.43000030517578
      },
      {
        "Date": "2007-04-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.86000061035156
      },
      {
        "Date": "2007-04-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.88999938964844
      },
      {
        "Date": "2007-04-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.849998474121094
      },
      {
        "Date": "2007-04-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.86000061035156
      },
      {
        "Date": "2007-04-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.06999969482422
      },
      {
        "Date": "2007-04-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.5099983215332
      },
      {
        "Date": "2007-04-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.279998779296875
      },
      {
        "Date": "2007-04-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.41999816894531
      },
      {
        "Date": "2007-04-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.22999954223633
      },
      {
        "Date": "2007-04-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.29999923706055
      },
      {
        "Date": "2007-04-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.81999969482422
      },
      {
        "Date": "2007-04-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.90999984741211
      },
      {
        "Date": "2007-04-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.040000915527344
      },
      {
        "Date": "2007-04-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.5099983215332
      },
      {
        "Date": "2007-04-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.619998931884766
      },
      {
        "Date": "2007-04-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.22999954223633
      },
      {
        "Date": "2007-04-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.720001220703125
      },
      {
        "Date": "2007-04-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.77000045776367
      },
      {
        "Date": "2007-04-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.900001525878906
      },
      {
        "Date": "2007-05-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.93000030517578
      },
      {
        "Date": "2007-05-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.0099983215332
      },
      {
        "Date": "2007-05-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.22999954223633
      },
      {
        "Date": "2007-05-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.2400016784668
      },
      {
        "Date": "2007-05-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.41999816894531
      },
      {
        "Date": "2007-05-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.400001525878906
      },
      {
        "Date": "2007-05-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.45000076293945
      },
      {
        "Date": "2007-05-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.58000183105469
      },
      {
        "Date": "2007-05-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.95000076293945
      },
      {
        "Date": "2007-05-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.779998779296875
      },
      {
        "Date": "2007-05-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.939998626708984
      },
      {
        "Date": "2007-05-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.119998931884766
      },
      {
        "Date": "2007-05-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.130001068115234
      },
      {
        "Date": "2007-05-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.279998779296875
      },
      {
        "Date": "2007-05-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.22999954223633
      },
      {"Date": "2007-05-22T00:00:00", "Bank": "BAC", "Stock Price": 51.5},
      {
        "Date": "2007-05-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.349998474121094
      },
      {
        "Date": "2007-05-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.04999923706055
      },
      {
        "Date": "2007-05-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.20000076293945
      },
      {
        "Date": "2007-05-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.189998626708984
      },
      {
        "Date": "2007-05-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.810001373291016
      },
      {
        "Date": "2007-05-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.709999084472656
      },
      {
        "Date": "2007-06-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.779998779296875
      },
      {
        "Date": "2007-06-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.849998474121094
      },
      {
        "Date": "2007-06-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.65999984741211
      },
      {
        "Date": "2007-06-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.33000183105469
      },
      {
        "Date": "2007-06-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.790000915527344
      },
      {
        "Date": "2007-06-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.2599983215332
      },
      {
        "Date": "2007-06-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.04999923706055
      },
      {
        "Date": "2007-06-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.65999984741211
      },
      {
        "Date": "2007-06-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.36000061035156
      },
      {
        "Date": "2007-06-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.08000183105469
      },
      {
        "Date": "2007-06-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.08000183105469
      },
      {
        "Date": "2007-06-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.90999984741211
      },
      {
        "Date": "2007-06-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.54999923706055
      },
      {
        "Date": "2007-06-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.97999954223633
      },
      {
        "Date": "2007-06-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.88999938964844
      },
      {
        "Date": "2007-06-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.95000076293945
      },
      {
        "Date": "2007-06-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.849998474121094
      },
      {
        "Date": "2007-06-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.79999923706055
      },
      {
        "Date": "2007-06-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.189998626708984
      },
      {
        "Date": "2007-06-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.09000015258789
      },
      {
        "Date": "2007-06-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.88999938964844
      },
      {
        "Date": "2007-07-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.31999969482422
      },
      {
        "Date": "2007-07-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.54999923706055
      },
      {
        "Date": "2007-07-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.369998931884766
      },
      {
        "Date": "2007-07-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.150001525878906
      },
      {
        "Date": "2007-07-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.810001373291016
      },
      {
        "Date": "2007-07-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.36000061035156
      },
      {
        "Date": "2007-07-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.5099983215332
      },
      {
        "Date": "2007-07-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.529998779296875
      },
      {"Date": "2007-07-13T00:00:00", "Bank": "BAC", "Stock Price": 49.5},
      {
        "Date": "2007-07-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.619998931884766
      },
      {
        "Date": "2007-07-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.79999923706055
      },
      {
        "Date": "2007-07-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.36000061035156
      },
      {
        "Date": "2007-07-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.27000045776367
      },
      {
        "Date": "2007-07-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.310001373291016
      },
      {
        "Date": "2007-07-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.150001525878906
      },
      {
        "Date": "2007-07-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.150001525878906
      },
      {
        "Date": "2007-07-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.93000030517578
      },
      {
        "Date": "2007-07-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.22999954223633
      },
      {
        "Date": "2007-07-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.40999984741211
      },
      {
        "Date": "2007-07-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.70000076293945
      },
      {
        "Date": "2007-07-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.41999816894531
      },
      {
        "Date": "2007-08-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.630001068115234
      },
      {
        "Date": "2007-08-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.779998779296875
      },
      {"Date": "2007-08-03T00:00:00", "Bank": "BAC", "Stock Price": 47},
      {
        "Date": "2007-08-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.15999984741211
      },
      {
        "Date": "2007-08-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.66999816894531
      },
      {
        "Date": "2007-08-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.70000076293945
      },
      {
        "Date": "2007-08-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.349998474121094
      },
      {
        "Date": "2007-08-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.59000015258789
      },
      {"Date": "2007-08-13T00:00:00", "Bank": "BAC", "Stock Price": 48.5},
      {
        "Date": "2007-08-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.86000061035156
      },
      {
        "Date": "2007-08-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.22999954223633
      },
      {
        "Date": "2007-08-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.849998474121094
      },
      {
        "Date": "2007-08-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.7599983215332
      },
      {
        "Date": "2007-08-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.349998474121094
      },
      {
        "Date": "2007-08-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.29999923706055
      },
      {
        "Date": "2007-08-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.650001525878906
      },
      {
        "Date": "2007-08-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.83000183105469
      },
      {
        "Date": "2007-08-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.869998931884766
      },
      {
        "Date": "2007-08-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.869998931884766
      },
      {
        "Date": "2007-08-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.65999984741211
      },
      {
        "Date": "2007-08-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.54999923706055
      },
      {
        "Date": "2007-08-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.209999084472656
      },
      {
        "Date": "2007-08-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.68000030517578
      },
      {
        "Date": "2007-09-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.08000183105469
      },
      {
        "Date": "2007-09-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.95000076293945
      },
      {
        "Date": "2007-09-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.790000915527344
      },
      {
        "Date": "2007-09-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.02000045776367
      },
      {
        "Date": "2007-09-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.959999084472656
      },
      {
        "Date": "2007-09-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.45000076293945
      },
      {
        "Date": "2007-09-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.38999938964844
      },
      {
        "Date": "2007-09-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.86000061035156
      },
      {
        "Date": "2007-09-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.95000076293945
      },
      {
        "Date": "2007-09-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 49.5099983215332
      },
      {
        "Date": "2007-09-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.209999084472656
      },
      {
        "Date": "2007-09-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.06999969482422
      },
      {
        "Date": "2007-09-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.790000915527344
      },
      {
        "Date": "2007-09-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.2400016784668
      },
      {
        "Date": "2007-09-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.59000015258789
      },
      {
        "Date": "2007-09-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.220001220703125
      },
      {
        "Date": "2007-09-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.40999984741211
      },
      {
        "Date": "2007-09-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.599998474121094
      },
      {
        "Date": "2007-09-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.27000045776367
      },
      {
        "Date": "2007-10-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.63999938964844
      },
      {
        "Date": "2007-10-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.720001220703125
      },
      {
        "Date": "2007-10-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.93000030517578
      },
      {
        "Date": "2007-10-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.400001525878906
      },
      {
        "Date": "2007-10-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.709999084472656
      },
      {
        "Date": "2007-10-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.43000030517578
      },
      {
        "Date": "2007-10-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.56999969482422
      },
      {
        "Date": "2007-10-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.29999923706055
      },
      {
        "Date": "2007-10-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.41999816894531
      },
      {
        "Date": "2007-10-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 52.06999969482422
      },
      {
        "Date": "2007-10-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 51.41999816894531
      },
      {
        "Date": "2007-10-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.20000076293945
      },
      {
        "Date": "2007-10-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 50.029998779296875
      },
      {
        "Date": "2007-10-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.849998474121094
      },
      {
        "Date": "2007-10-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.56999969482422
      },
      {
        "Date": "2007-10-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.779998779296875
      },
      {
        "Date": "2007-10-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.779998779296875
      },
      {
        "Date": "2007-10-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.47999954223633
      },
      {"Date": "2007-10-25T00:00:00", "Bank": "BAC", "Stock Price": 47},
      {
        "Date": "2007-10-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.029998779296875
      },
      {
        "Date": "2007-10-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.97999954223633
      },
      {
        "Date": "2007-10-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 47.9900016784668
      },
      {
        "Date": "2007-10-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 48.279998779296875
      },
      {
        "Date": "2007-11-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.709999084472656
      },
      {
        "Date": "2007-11-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.11000061035156
      },
      {
        "Date": "2007-11-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.45000076293945
      },
      {
        "Date": "2007-11-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.560001373291016
      },
      {
        "Date": "2007-11-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.310001373291016
      },
      {"Date": "2007-11-08T00:00:00", "Bank": "BAC", "Stock Price": 43.5},
      {
        "Date": "2007-11-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.97999954223633
      },
      {
        "Date": "2007-11-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.97999954223633
      },
      {
        "Date": "2007-11-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 46.27000045776367
      },
      {
        "Date": "2007-11-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.72999954223633
      },
      {
        "Date": "2007-11-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.08000183105469
      },
      {
        "Date": "2007-11-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.369998931884766
      },
      {
        "Date": "2007-11-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.81999969482422
      },
      {
        "Date": "2007-11-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.77000045776367
      },
      {
        "Date": "2007-11-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.13999938964844
      },
      {
        "Date": "2007-11-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.150001525878906
      },
      {
        "Date": "2007-11-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.880001068115234
      },
      {
        "Date": "2007-11-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.939998626708984
      },
      {
        "Date": "2007-11-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.849998474121094
      },
      {
        "Date": "2007-11-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.630001068115234
      },
      {
        "Date": "2007-11-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 46.130001068115234
      },
      {
        "Date": "2007-12-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.470001220703125
      },
      {
        "Date": "2007-12-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.709999084472656
      },
      {
        "Date": "2007-12-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.22999954223633
      },
      {
        "Date": "2007-12-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.959999084472656
      },
      {
        "Date": "2007-12-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.369998931884766
      },
      {
        "Date": "2007-12-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 46.63999938964844
      },
      {
        "Date": "2007-12-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.650001525878906
      },
      {
        "Date": "2007-12-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.43000030517578
      },
      {
        "Date": "2007-12-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.04999923706055
      },
      {
        "Date": "2007-12-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.15999984741211
      },
      {
        "Date": "2007-12-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.70000076293945
      },
      {"Date": "2007-12-18T00:00:00", "Bank": "BAC", "Stock Price": 41.5},
      {
        "Date": "2007-12-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.59000015258789
      },
      {
        "Date": "2007-12-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.40999984741211
      },
      {
        "Date": "2007-12-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.91999816894531
      },
      {
        "Date": "2007-12-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.279998779296875
      },
      {
        "Date": "2007-12-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.29999923706055
      },
      {
        "Date": "2007-12-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.459999084472656
      },
      {
        "Date": "2007-12-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.099998474121094
      },
      {
        "Date": "2007-12-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.2599983215332
      },
      {
        "Date": "2008-01-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 40.560001373291016
      },
      {
        "Date": "2008-01-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 40.29999923706055
      },
      {
        "Date": "2008-01-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.849998474121094
      },
      {
        "Date": "2008-01-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2008-01-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.40999984741211
      },
      {
        "Date": "2008-01-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.7400016784668
      },
      {
        "Date": "2008-01-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.29999923706055
      },
      {"Date": "2008-01-11T00:00:00", "Bank": "BAC", "Stock Price": 38.5},
      {
        "Date": "2008-01-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.220001220703125
      },
      {
        "Date": "2008-01-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.880001068115234
      },
      {
        "Date": "2008-01-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.689998626708984
      },
      {
        "Date": "2008-01-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.90999984741211
      },
      {
        "Date": "2008-01-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 35.970001220703125
      },
      {
        "Date": "2008-01-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.38999938964844
      },
      {
        "Date": "2008-01-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 40.56999969482422
      },
      {
        "Date": "2008-01-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2008-01-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.47999954223633
      },
      {
        "Date": "2008-01-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.20000076293945
      },
      {
        "Date": "2008-01-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.939998626708984
      },
      {
        "Date": "2008-01-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.209999084472656
      },
      {
        "Date": "2008-01-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.150001525878906
      },
      {
        "Date": "2008-02-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 45.029998779296875
      },
      {
        "Date": "2008-02-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 44.029998779296875
      },
      {
        "Date": "2008-02-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.369998931884766
      },
      {
        "Date": "2008-02-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.33000183105469
      },
      {
        "Date": "2008-02-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.369998931884766
      },
      {
        "Date": "2008-02-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.15999984741211
      },
      {
        "Date": "2008-02-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.13999938964844
      },
      {
        "Date": "2008-02-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.81999969482422
      },
      {
        "Date": "2008-02-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 43.33000183105469
      },
      {
        "Date": "2008-02-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.2400016784668
      },
      {
        "Date": "2008-02-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.70000076293945
      },
      {
        "Date": "2008-02-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.66999816894531
      },
      {
        "Date": "2008-02-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.970001220703125
      },
      {
        "Date": "2008-02-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.209999084472656
      },
      {
        "Date": "2008-02-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.599998474121094
      },
      {
        "Date": "2008-02-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.939998626708984
      },
      {
        "Date": "2008-02-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.720001220703125
      },
      {
        "Date": "2008-02-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.880001068115234
      },
      {
        "Date": "2008-02-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.41999816894531
      },
      {
        "Date": "2008-02-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.7400016784668
      },
      {
        "Date": "2008-03-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.18000030517578
      },
      {
        "Date": "2008-03-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.779998779296875
      },
      {
        "Date": "2008-03-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.54999923706055
      },
      {
        "Date": "2008-03-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.52000045776367
      },
      {
        "Date": "2008-03-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.7400016784668
      },
      {
        "Date": "2008-03-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 35.310001373291016
      },
      {
        "Date": "2008-03-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.720001220703125
      },
      {
        "Date": "2008-03-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.029998779296875
      },
      {
        "Date": "2008-03-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.13999938964844
      },
      {
        "Date": "2008-03-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 35.689998626708984
      },
      {
        "Date": "2008-03-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 35.959999084472656
      },
      {
        "Date": "2008-03-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.93000030517578
      },
      {
        "Date": "2008-03-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.560001373291016
      },
      {
        "Date": "2008-03-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 41.86000061035156
      },
      {
        "Date": "2008-03-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 42.45000076293945
      },
      {
        "Date": "2008-03-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 40.970001220703125
      },
      {
        "Date": "2008-03-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.84000015258789
      },
      {
        "Date": "2008-03-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.63999938964844
      },
      {
        "Date": "2008-03-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.06999969482422
      },
      {
        "Date": "2008-03-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.90999984741211
      },
      {
        "Date": "2008-04-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 40.86000061035156
      },
      {
        "Date": "2008-04-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 40.29999923706055
      },
      {
        "Date": "2008-04-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 40.369998931884766
      },
      {
        "Date": "2008-04-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.40999984741211
      },
      {"Date": "2008-04-07T00:00:00", "Bank": "BAC", "Stock Price": 39.5},
      {
        "Date": "2008-04-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.380001068115234
      },
      {
        "Date": "2008-04-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.93000030517578
      },
      {
        "Date": "2008-04-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.689998626708984
      },
      {
        "Date": "2008-04-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.939998626708984
      },
      {
        "Date": "2008-04-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 35.58000183105469
      },
      {
        "Date": "2008-04-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 35.58000183105469
      },
      {
        "Date": "2008-04-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.97999954223633
      },
      {
        "Date": "2008-04-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.470001220703125
      },
      {
        "Date": "2008-04-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.560001373291016
      },
      {
        "Date": "2008-04-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.61000061035156
      },
      {"Date": "2008-04-22T00:00:00", "Bank": "BAC", "Stock Price": 37},
      {
        "Date": "2008-04-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.86000061035156
      },
      {
        "Date": "2008-04-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.869998931884766
      },
      {
        "Date": "2008-04-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.29999923706055
      },
      {
        "Date": "2008-04-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.18000030517578
      },
      {
        "Date": "2008-04-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.86000061035156
      },
      {
        "Date": "2008-04-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.540000915527344
      },
      {
        "Date": "2008-05-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.38999938964844
      },
      {
        "Date": "2008-05-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.790000915527344
      },
      {
        "Date": "2008-05-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.970001220703125
      },
      {
        "Date": "2008-05-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 39.2400016784668
      },
      {"Date": "2008-05-07T00:00:00", "Bank": "BAC", "Stock Price": 38},
      {
        "Date": "2008-05-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.33000183105469
      },
      {
        "Date": "2008-05-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.650001525878906
      },
      {
        "Date": "2008-05-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.439998626708984
      },
      {
        "Date": "2008-05-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.61000061035156
      },
      {
        "Date": "2008-05-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.79999923706055
      },
      {
        "Date": "2008-05-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.709999084472656
      },
      {
        "Date": "2008-05-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.16999816894531
      },
      {
        "Date": "2008-05-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.099998474121094
      },
      {
        "Date": "2008-05-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 35.38999938964844
      },
      {
        "Date": "2008-05-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.630001068115234
      },
      {
        "Date": "2008-05-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.72999954223633
      },
      {
        "Date": "2008-05-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.93000030517578
      },
      {
        "Date": "2008-05-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.16999816894531
      },
      {
        "Date": "2008-05-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.869998931884766
      },
      {
        "Date": "2008-05-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.599998474121094
      },
      {
        "Date": "2008-05-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.0099983215332
      },
      {
        "Date": "2008-06-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.58000183105469
      },
      {
        "Date": "2008-06-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.310001373291016
      },
      {
        "Date": "2008-06-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 31.989999771118164
      },
      {
        "Date": "2008-06-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 31.989999771118164
      },
      {"Date": "2008-06-06T00:00:00", "Bank": "BAC", "Stock Price": 30.5},
      {
        "Date": "2008-06-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.610000610351562
      },
      {
        "Date": "2008-06-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.6200008392334
      },
      {
        "Date": "2008-06-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.850000381469727
      },
      {
        "Date": "2008-06-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.440000534057617
      },
      {
        "Date": "2008-06-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.780000686645508
      },
      {
        "Date": "2008-06-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 30.31999969482422
      },
      {
        "Date": "2008-06-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.239999771118164
      },
      {
        "Date": "2008-06-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.3700008392334
      },
      {
        "Date": "2008-06-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.139999389648438
      },
      {
        "Date": "2008-06-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 27.100000381469727
      },
      {
        "Date": "2008-06-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 25.8799991607666
      },
      {
        "Date": "2008-06-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 26.6200008392334
      },
      {
        "Date": "2008-06-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 26.610000610351562
      },
      {
        "Date": "2008-06-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 24.809999465942383
      },
      {
        "Date": "2008-06-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 24.59000015258789
      },
      {
        "Date": "2008-06-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.8700008392334
      },
      {
        "Date": "2008-07-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.809999465942383
      },
      {
        "Date": "2008-07-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.540000915527344
      },
      {
        "Date": "2008-07-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.399999618530273
      },
      {
        "Date": "2008-07-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 21.530000686645508
      },
      {
        "Date": "2008-07-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.540000915527344
      },
      {
        "Date": "2008-07-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.059999465942383
      },
      {
        "Date": "2008-07-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.360000610351562
      },
      {
        "Date": "2008-07-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 21.670000076293945
      },
      {
        "Date": "2008-07-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 20.149999618530273
      },
      {
        "Date": "2008-07-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.520000457763672
      },
      {
        "Date": "2008-07-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.670000076293945
      },
      {"Date": "2008-07-17T00:00:00", "Bank": "BAC", "Stock Price": 26.5},
      {
        "Date": "2008-07-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 27.489999771118164
      },
      {
        "Date": "2008-07-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.559999465942383
      },
      {
        "Date": "2008-07-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.349998474121094
      },
      {
        "Date": "2008-07-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.439998626708984
      },
      {
        "Date": "2008-07-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 30.639999389648438
      },
      {
        "Date": "2008-07-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.579999923706055
      },
      {
        "Date": "2008-07-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.059999465942383
      },
      {
        "Date": "2008-07-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.220001220703125
      },
      {
        "Date": "2008-07-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.61000061035156
      },
      {
        "Date": "2008-07-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.900001525878906
      },
      {
        "Date": "2008-08-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.33000183105469
      },
      {
        "Date": "2008-08-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.619998931884766
      },
      {
        "Date": "2008-08-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.58000183105469
      },
      {
        "Date": "2008-08-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.45000076293945
      },
      {
        "Date": "2008-08-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 31.520000457763672
      },
      {"Date": "2008-08-08T00:00:00", "Bank": "BAC", "Stock Price": 32.25},
      {
        "Date": "2008-08-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.380001068115234
      },
      {
        "Date": "2008-08-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 31.1299991607666
      },
      {
        "Date": "2008-08-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.860000610351562
      },
      {
        "Date": "2008-08-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 30.18000030517578
      },
      {
        "Date": "2008-08-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 30.700000762939453
      },
      {
        "Date": "2008-08-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.299999237060547
      },
      {
        "Date": "2008-08-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.079999923706055
      },
      {
        "Date": "2008-08-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.290000915527344
      },
      {
        "Date": "2008-08-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.040000915527344
      },
      {
        "Date": "2008-08-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 30.209999084472656
      },
      {
        "Date": "2008-08-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 28.959999084472656
      },
      {
        "Date": "2008-08-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.020000457763672
      },
      {
        "Date": "2008-08-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.649999618530273
      },
      {
        "Date": "2008-08-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 31.43000030517578
      },
      {
        "Date": "2008-08-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 31.139999389648438
      },
      {
        "Date": "2008-09-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.630001068115234
      },
      {
        "Date": "2008-09-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.959999084472656
      },
      {
        "Date": "2008-09-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 30.600000381469727
      },
      {
        "Date": "2008-09-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.22999954223633
      },
      {
        "Date": "2008-09-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.72999954223633
      },
      {
        "Date": "2008-09-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.52000045776367
      },
      {
        "Date": "2008-09-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.400001525878906
      },
      {
        "Date": "2008-09-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.060001373291016
      },
      {
        "Date": "2008-09-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.7400016784668
      },
      {
        "Date": "2008-09-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 26.549999237060547
      },
      {
        "Date": "2008-09-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 29.549999237060547
      },
      {
        "Date": "2008-09-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 27.200000762939453
      },
      {
        "Date": "2008-09-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 30.579999923706055
      },
      {
        "Date": "2008-09-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 37.47999954223633
      },
      {
        "Date": "2008-09-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.150001525878906
      },
      {
        "Date": "2008-09-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.29999923706055
      },
      {
        "Date": "2008-09-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 33.06999969482422
      },
      {
        "Date": "2008-09-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.369998931884766
      },
      {
        "Date": "2008-09-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.70000076293945
      },
      {"Date": "2008-09-29T00:00:00", "Bank": "BAC", "Stock Price": 30.25},
      {"Date": "2008-09-30T00:00:00", "Bank": "BAC", "Stock Price": 35},
      {
        "Date": "2008-10-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 38.130001068115234
      },
      {
        "Date": "2008-10-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 36.369998931884766
      },
      {
        "Date": "2008-10-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 34.47999954223633
      },
      {
        "Date": "2008-10-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 32.220001220703125
      },
      {
        "Date": "2008-10-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.770000457763672
      },
      {
        "Date": "2008-10-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.100000381469727
      },
      {
        "Date": "2008-10-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 19.6299991607666
      },
      {
        "Date": "2008-10-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 20.8700008392334
      },
      {
        "Date": "2008-10-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.790000915527344
      },
      {
        "Date": "2008-10-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 26.530000686645508
      },
      {
        "Date": "2008-10-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.81999969482422
      },
      {"Date": "2008-10-16T00:00:00", "Bank": "BAC", "Stock Price": 24.25},
      {
        "Date": "2008-10-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.239999771118164
      },
      {
        "Date": "2008-10-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 24.399999618530273
      },
      {
        "Date": "2008-10-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.969999313354492
      },
      {
        "Date": "2008-10-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.65999984741211
      },
      {"Date": "2008-10-23T00:00:00", "Bank": "BAC", "Stock Price": 23},
      {
        "Date": "2008-10-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 21.06999969482422
      },
      {
        "Date": "2008-10-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 20.530000686645508
      },
      {
        "Date": "2008-10-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.020000457763672
      },
      {
        "Date": "2008-10-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.31999969482422
      },
      {
        "Date": "2008-10-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 22.780000686645508
      },
      {
        "Date": "2008-10-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 24.170000076293945
      },
      {
        "Date": "2008-11-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 23.610000610351562
      },
      {
        "Date": "2008-11-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 24.530000686645508
      },
      {"Date": "2008-11-05T00:00:00", "Bank": "BAC", "Stock Price": 21.75},
      {
        "Date": "2008-11-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 20.1200008392334
      },
      {
        "Date": "2008-11-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 20.489999771118164
      },
      {
        "Date": "2008-11-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 19.479999542236328
      },
      {
        "Date": "2008-11-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.690000534057617
      },
      {"Date": "2008-11-12T00:00:00", "Bank": "BAC", "Stock Price": 17},
      {
        "Date": "2008-11-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.100000381469727
      },
      {
        "Date": "2008-11-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.420000076293945
      },
      {
        "Date": "2008-11-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.029999732971191
      },
      {
        "Date": "2008-11-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.1899995803833
      },
      {
        "Date": "2008-11-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.0600004196167
      },
      {"Date": "2008-11-20T00:00:00", "Bank": "BAC", "Stock Price": 11.25},
      {
        "Date": "2008-11-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.470000267028809
      },
      {
        "Date": "2008-11-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.59000015258789
      },
      {
        "Date": "2008-11-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.800000190734863
      },
      {
        "Date": "2008-11-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.430000305175781
      },
      {"Date": "2008-11-28T00:00:00", "Bank": "BAC", "Stock Price": 16.25},
      {
        "Date": "2008-12-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.850000381469727
      },
      {
        "Date": "2008-12-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.369999885559082
      },
      {
        "Date": "2008-12-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.050000190734863
      },
      {
        "Date": "2008-12-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.34000015258789
      },
      {
        "Date": "2008-12-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.239999771118164
      },
      {
        "Date": "2008-12-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.84000015258789
      },
      {
        "Date": "2008-12-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.950000762939453
      },
      {
        "Date": "2008-12-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.690000534057617
      },
      {
        "Date": "2008-12-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.90999984741211
      },
      {
        "Date": "2008-12-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.930000305175781
      },
      {
        "Date": "2008-12-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.109999656677246
      },
      {
        "Date": "2008-12-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.100000381469727
      },
      {
        "Date": "2008-12-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.619999885559082
      },
      {
        "Date": "2008-12-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.960000038146973
      },
      {
        "Date": "2008-12-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.800000190734863
      },
      {
        "Date": "2008-12-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.529999732971191
      },
      {"Date": "2008-12-23T00:00:00", "Bank": "BAC", "Stock Price": 12.75},
      {
        "Date": "2008-12-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.529999732971191
      },
      {
        "Date": "2008-12-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.359999656677246
      },
      {
        "Date": "2008-12-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.9399995803833
      },
      {
        "Date": "2008-12-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.239999771118164
      },
      {
        "Date": "2008-12-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.079999923706055
      },
      {
        "Date": "2009-01-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.329999923706055
      },
      {
        "Date": "2009-01-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.979999542236328
      },
      {
        "Date": "2009-01-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.279999732971191
      },
      {
        "Date": "2009-01-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.710000038146973
      },
      {
        "Date": "2009-01-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.539999961853027
      },
      {
        "Date": "2009-01-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.989999771118164
      },
      {
        "Date": "2009-01-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.430000305175781
      },
      {
        "Date": "2009-01-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.649999618530273
      },
      {
        "Date": "2009-01-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.199999809265137
      },
      {
        "Date": "2009-01-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.319999694824219
      },
      {
        "Date": "2009-01-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.179999828338623
      },
      {
        "Date": "2009-01-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.099999904632568
      },
      {
        "Date": "2009-01-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.679999828338623
      },
      {
        "Date": "2009-01-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.710000038146973
      },
      {
        "Date": "2009-01-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.239999771118164
      },
      {"Date": "2009-01-26T00:00:00", "Bank": "BAC", "Stock Price": 6},
      {"Date": "2009-01-27T00:00:00", "Bank": "BAC", "Stock Price": 6.5},
      {
        "Date": "2009-01-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.389999866485596
      },
      {
        "Date": "2009-01-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.78000020980835
      },
      {
        "Date": "2009-01-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.579999923706055
      },
      {"Date": "2009-02-02T00:00:00", "Bank": "BAC", "Stock Price": 6},
      {
        "Date": "2009-02-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.300000190734863
      },
      {
        "Date": "2009-02-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 4.699999809265137
      },
      {
        "Date": "2009-02-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 4.840000152587891
      },
      {
        "Date": "2009-02-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.130000114440918
      },
      {
        "Date": "2009-02-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.889999866485596
      },
      {
        "Date": "2009-02-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.559999942779541
      },
      {
        "Date": "2009-02-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.070000171661377
      },
      {
        "Date": "2009-02-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.869999885559082
      },
      {
        "Date": "2009-02-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.570000171661377
      },
      {
        "Date": "2009-02-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 4.900000095367432
      },
      {
        "Date": "2009-02-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 4.570000171661377
      },
      {
        "Date": "2009-02-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.930000066757202
      },
      {
        "Date": "2009-02-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.7899999618530273
      },
      {
        "Date": "2009-02-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.9100000858306885
      },
      {
        "Date": "2009-02-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 4.730000019073486
      },
      {
        "Date": "2009-02-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.159999847412109
      },
      {
        "Date": "2009-02-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.320000171661377
      },
      {
        "Date": "2009-02-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.950000047683716
      },
      {
        "Date": "2009-03-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.630000114440918
      },
      {
        "Date": "2009-03-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.6500000953674316
      },
      {
        "Date": "2009-03-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.5899999141693115
      },
      {
        "Date": "2009-03-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.1700000762939453
      },
      {
        "Date": "2009-03-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 3.140000104904175
      },
      {"Date": "2009-03-09T00:00:00", "Bank": "BAC", "Stock Price": 3.75},
      {
        "Date": "2009-03-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 4.789999961853027
      },
      {
        "Date": "2009-03-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 4.929999828338623
      },
      {
        "Date": "2009-03-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.849999904632568
      },
      {
        "Date": "2009-03-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 5.760000228881836
      },
      {
        "Date": "2009-03-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.179999828338623
      },
      {
        "Date": "2009-03-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.269999980926514
      },
      {
        "Date": "2009-03-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.670000076293945
      },
      {
        "Date": "2009-03-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.929999828338623
      },
      {
        "Date": "2009-03-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.190000057220459
      },
      {
        "Date": "2009-03-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.800000190734863
      },
      {
        "Date": "2009-03-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.21999979019165
      },
      {
        "Date": "2009-03-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.699999809265137
      },
      {
        "Date": "2009-03-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.579999923706055
      },
      {
        "Date": "2009-03-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.340000152587891
      },
      {
        "Date": "2009-03-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.03000020980835
      },
      {
        "Date": "2009-03-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 6.820000171661377
      },
      {
        "Date": "2009-04-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.050000190734863
      },
      {
        "Date": "2009-04-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.239999771118164
      },
      {
        "Date": "2009-04-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.599999904632568
      },
      {
        "Date": "2009-04-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.480000019073486
      },
      {
        "Date": "2009-04-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.360000133514404
      },
      {
        "Date": "2009-04-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 7.059999942779541
      },
      {
        "Date": "2009-04-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 9.550000190734863
      },
      {
        "Date": "2009-04-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.020000457763672
      },
      {
        "Date": "2009-04-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.09000015258789
      },
      {
        "Date": "2009-04-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.4399995803833
      },
      {
        "Date": "2009-04-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.34000015258789
      },
      {
        "Date": "2009-04-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.600000381469727
      },
      {
        "Date": "2009-04-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.020000457763672
      },
      {
        "Date": "2009-04-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.760000228881836
      },
      {
        "Date": "2009-04-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.260000228881836
      },
      {
        "Date": "2009-04-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.819999694824219
      },
      {
        "Date": "2009-04-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 9.100000381469727
      },
      {
        "Date": "2009-04-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.920000076293945
      },
      {
        "Date": "2009-04-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.149999618530273
      },
      {
        "Date": "2009-04-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.680000305175781
      },
      {
        "Date": "2009-04-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.930000305175781
      },
      {
        "Date": "2009-05-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 8.699999809265137
      },
      {
        "Date": "2009-05-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.380000114440918
      },
      {
        "Date": "2009-05-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.84000015258789
      },
      {
        "Date": "2009-05-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.6899995803833
      },
      {
        "Date": "2009-05-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.510000228881836
      },
      {
        "Date": "2009-05-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.170000076293945
      },
      {
        "Date": "2009-05-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.9399995803833
      },
      {
        "Date": "2009-05-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.260000228881836
      },
      {
        "Date": "2009-05-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.010000228881836
      },
      {
        "Date": "2009-05-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.3100004196167
      },
      {
        "Date": "2009-05-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.670000076293945
      },
      {
        "Date": "2009-05-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.729999542236328
      },
      {"Date": "2009-05-19T00:00:00", "Bank": "BAC", "Stock Price": 11.25},
      {
        "Date": "2009-05-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.489999771118164
      },
      {
        "Date": "2009-05-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.40999984741211
      },
      {
        "Date": "2009-05-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.069999694824219
      },
      {
        "Date": "2009-05-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.979999542236328
      },
      {
        "Date": "2009-05-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.90999984741211
      },
      {
        "Date": "2009-05-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.300000190734863
      },
      {
        "Date": "2009-05-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.270000457763672
      },
      {
        "Date": "2009-06-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.210000038146973
      },
      {
        "Date": "2009-06-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.40999984741211
      },
      {
        "Date": "2009-06-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.210000038146973
      },
      {
        "Date": "2009-06-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.869999885559082
      },
      {
        "Date": "2009-06-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.859999656677246
      },
      {
        "Date": "2009-06-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.0600004196167
      },
      {
        "Date": "2009-06-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.0600004196167
      },
      {
        "Date": "2009-06-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.979999542236328
      },
      {
        "Date": "2009-06-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.970000267028809
      },
      {
        "Date": "2009-06-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.720000267028809
      },
      {
        "Date": "2009-06-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.329999923706055
      },
      {
        "Date": "2009-06-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.729999542236328
      },
      {
        "Date": "2009-06-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.300000190734863
      },
      {
        "Date": "2009-06-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.899999618530273
      },
      {
        "Date": "2009-06-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.220000267028809
      },
      {
        "Date": "2009-06-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.9399995803833
      },
      {
        "Date": "2009-06-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.229999542236328
      },
      {
        "Date": "2009-06-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.350000381469727
      },
      {
        "Date": "2009-06-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.350000381469727
      },
      {"Date": "2009-06-26T00:00:00", "Bank": "BAC", "Stock Price": 12.75},
      {
        "Date": "2009-06-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.1899995803833
      },
      {
        "Date": "2009-06-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.199999809265137
      },
      {
        "Date": "2009-07-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.050000190734863
      },
      {
        "Date": "2009-07-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.640000343322754
      },
      {
        "Date": "2009-07-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.149999618530273
      },
      {
        "Date": "2009-07-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.149999618530273
      },
      {
        "Date": "2009-07-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.84000015258789
      },
      {
        "Date": "2009-07-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.970000267028809
      },
      {
        "Date": "2009-07-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.880000114440918
      },
      {
        "Date": "2009-07-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.989999771118164
      },
      {
        "Date": "2009-07-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.90999984741211
      },
      {
        "Date": "2009-07-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.420000076293945
      },
      {
        "Date": "2009-07-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.170000076293945
      },
      {
        "Date": "2009-07-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.890000343322754
      },
      {
        "Date": "2009-07-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.239999771118164
      },
      {
        "Date": "2009-07-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.1899995803833
      },
      {
        "Date": "2009-07-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.229999542236328
      },
      {
        "Date": "2009-07-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.6899995803833
      },
      {
        "Date": "2009-07-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.510000228881836
      },
      {
        "Date": "2009-07-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.09000015258789
      },
      {
        "Date": "2009-07-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.34000015258789
      },
      {
        "Date": "2009-07-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.520000457763672
      },
      {
        "Date": "2009-07-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.970000267028809
      },
      {
        "Date": "2009-07-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.789999961853027
      },
      {
        "Date": "2009-08-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.319999694824219
      },
      {
        "Date": "2009-08-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.640000343322754
      },
      {
        "Date": "2009-08-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.65999984741211
      },
      {
        "Date": "2009-08-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.700000762939453
      },
      {
        "Date": "2009-08-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.420000076293945
      },
      {
        "Date": "2009-08-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.68000030517578
      },
      {
        "Date": "2009-08-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.850000381469727
      },
      {
        "Date": "2009-08-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.930000305175781
      },
      {"Date": "2009-08-13T00:00:00", "Bank": "BAC", "Stock Price": 17},
      {
        "Date": "2009-08-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.389999389648438
      },
      {
        "Date": "2009-08-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.559999465942383
      },
      {
        "Date": "2009-08-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.899999618530273
      },
      {"Date": "2009-08-19T00:00:00", "Bank": "BAC", "Stock Price": 16.75},
      {
        "Date": "2009-08-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.139999389648438
      },
      {
        "Date": "2009-08-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.459999084472656
      },
      {
        "Date": "2009-08-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.350000381469727
      },
      {"Date": "2009-08-25T00:00:00", "Bank": "BAC", "Stock Price": 17.75},
      {
        "Date": "2009-08-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.790000915527344
      },
      {
        "Date": "2009-08-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.920000076293945
      },
      {
        "Date": "2009-08-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.979999542236328
      },
      {
        "Date": "2009-08-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.59000015258789
      },
      {
        "Date": "2009-09-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.459999084472656
      },
      {
        "Date": "2009-09-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.270000457763672
      },
      {
        "Date": "2009-09-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.84000015258789
      },
      {
        "Date": "2009-09-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.09000015258789
      },
      {
        "Date": "2009-09-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.020000457763672
      },
      {
        "Date": "2009-09-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.040000915527344
      },
      {
        "Date": "2009-09-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.219999313354492
      },
      {
        "Date": "2009-09-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.969999313354492
      },
      {
        "Date": "2009-09-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.989999771118164
      },
      {
        "Date": "2009-09-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.790000915527344
      },
      {"Date": "2009-09-16T00:00:00", "Bank": "BAC", "Stock Price": 17.25},
      {
        "Date": "2009-09-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.610000610351562
      },
      {
        "Date": "2009-09-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.6299991607666
      },
      {"Date": "2009-09-21T00:00:00", "Bank": "BAC", "Stock Price": 17.25},
      {
        "Date": "2009-09-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.610000610351562
      },
      {"Date": "2009-09-23T00:00:00", "Bank": "BAC", "Stock Price": 17.5},
      {
        "Date": "2009-09-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.979999542236328
      },
      {
        "Date": "2009-09-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.600000381469727
      },
      {
        "Date": "2009-09-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.219999313354492
      },
      {
        "Date": "2009-09-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.15999984741211
      },
      {
        "Date": "2009-09-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.920000076293945
      },
      {
        "Date": "2009-10-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.209999084472656
      },
      {
        "Date": "2009-10-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.34000015258789
      },
      {
        "Date": "2009-10-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.959999084472656
      },
      {"Date": "2009-10-06T00:00:00", "Bank": "BAC", "Stock Price": 17},
      {
        "Date": "2009-10-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.350000381469727
      },
      {
        "Date": "2009-10-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.329999923706055
      },
      {"Date": "2009-10-09T00:00:00", "Bank": "BAC", "Stock Price": 17.5},
      {
        "Date": "2009-10-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.030000686645508
      },
      {
        "Date": "2009-10-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.809999465942383
      },
      {
        "Date": "2009-10-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.59000015258789
      },
      {
        "Date": "2009-10-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.100000381469727
      },
      {
        "Date": "2009-10-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.260000228881836
      },
      {
        "Date": "2009-10-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.15999984741211
      },
      {
        "Date": "2009-10-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.010000228881836
      },
      {
        "Date": "2009-10-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.510000228881836
      },
      {
        "Date": "2009-10-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.520000457763672
      },
      {
        "Date": "2009-10-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.219999313354492
      },
      {
        "Date": "2009-10-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.399999618530273
      },
      {
        "Date": "2009-10-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.449999809265137
      },
      {
        "Date": "2009-10-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.010000228881836
      },
      {
        "Date": "2009-10-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.729999542236328
      },
      {
        "Date": "2009-10-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.579999923706055
      },
      {
        "Date": "2009-11-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.630000114440918
      },
      {
        "Date": "2009-11-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.800000190734863
      },
      {
        "Date": "2009-11-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.699999809265137
      },
      {
        "Date": "2009-11-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.130000114440918
      },
      {
        "Date": "2009-11-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.050000190734863
      },
      {
        "Date": "2009-11-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.770000457763672
      },
      {
        "Date": "2009-11-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.030000686645508
      },
      {
        "Date": "2009-11-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.43000030517578
      },
      {
        "Date": "2009-11-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.059999465942383
      },
      {
        "Date": "2009-11-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.979999542236328
      },
      {
        "Date": "2009-11-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.869999885559082
      },
      {
        "Date": "2009-11-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.770000457763672
      },
      {
        "Date": "2009-11-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.350000381469727
      },
      {
        "Date": "2009-11-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.079999923706055
      },
      {
        "Date": "2009-11-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.09000015258789
      },
      {
        "Date": "2009-11-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.290000915527344
      },
      {
        "Date": "2009-11-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.100000381469727
      },
      {
        "Date": "2009-11-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.949999809265137
      },
      {
        "Date": "2009-11-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.470000267028809
      },
      {
        "Date": "2009-11-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.850000381469727
      },
      {
        "Date": "2009-12-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.899999618530273
      },
      {
        "Date": "2009-12-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.649999618530273
      },
      {
        "Date": "2009-12-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.760000228881836
      },
      {
        "Date": "2009-12-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.280000686645508
      },
      {
        "Date": "2009-12-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.890000343322754
      },
      {
        "Date": "2009-12-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.40999984741211
      },
      {
        "Date": "2009-12-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.390000343322754
      },
      {
        "Date": "2009-12-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.210000038146973
      },
      {
        "Date": "2009-12-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.630000114440918
      },
      {
        "Date": "2009-12-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.630000114440918
      },
      {
        "Date": "2009-12-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.1899995803833
      },
      {
        "Date": "2009-12-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.279999732971191
      },
      {
        "Date": "2009-12-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.859999656677246
      },
      {
        "Date": "2009-12-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.029999732971191
      },
      {
        "Date": "2009-12-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.279999732971191
      },
      {
        "Date": "2009-12-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.329999923706055
      },
      {
        "Date": "2009-12-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.1899995803833
      },
      {"Date": "2009-12-24T00:00:00", "Bank": "BAC", "Stock Price": 15.25},
      {
        "Date": "2009-12-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.289999961853027
      },
      {
        "Date": "2009-12-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.119999885559082
      },
      {
        "Date": "2009-12-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.069999694824219
      },
      {
        "Date": "2009-12-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.0600004196167
      },
      {
        "Date": "2010-01-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.6899995803833
      },
      {
        "Date": "2010-01-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.200000762939453
      },
      {
        "Date": "2010-01-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.389999389648438
      },
      {
        "Date": "2010-01-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.93000030517578
      },
      {
        "Date": "2010-01-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.780000686645508
      },
      {
        "Date": "2010-01-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.93000030517578
      },
      {
        "Date": "2010-01-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.360000610351562
      },
      {
        "Date": "2010-01-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.6200008392334
      },
      {
        "Date": "2010-01-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.81999969482422
      },
      {
        "Date": "2010-01-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.260000228881836
      },
      {
        "Date": "2010-01-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.31999969482422
      },
      {
        "Date": "2010-01-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.489999771118164
      },
      {
        "Date": "2010-01-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.470000267028809
      },
      {
        "Date": "2010-01-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.899999618530273
      },
      {
        "Date": "2010-01-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.979999542236328
      },
      {
        "Date": "2010-01-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.770000457763672
      },
      {
        "Date": "2010-01-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.1899995803833
      },
      {
        "Date": "2010-01-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.369999885559082
      },
      {
        "Date": "2010-01-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.180000305175781
      },
      {
        "Date": "2010-02-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.420000076293945
      },
      {
        "Date": "2010-02-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.600000381469727
      },
      {
        "Date": "2010-02-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.529999732971191
      },
      {"Date": "2010-02-04T00:00:00", "Bank": "BAC", "Stock Price": 14.75},
      {"Date": "2010-02-05T00:00:00", "Bank": "BAC", "Stock Price": 15},
      {
        "Date": "2010-02-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.479999542236328
      },
      {
        "Date": "2010-02-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.470000267028809
      },
      {
        "Date": "2010-02-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.670000076293945
      },
      {
        "Date": "2010-02-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.630000114440918
      },
      {
        "Date": "2010-02-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.449999809265137
      },
      {
        "Date": "2010-02-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.15999984741211
      },
      {
        "Date": "2010-02-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.65999984741211
      },
      {
        "Date": "2010-02-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.880000114440918
      },
      {
        "Date": "2010-02-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.880000114440918
      },
      {
        "Date": "2010-02-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.209999084472656
      },
      {
        "Date": "2010-02-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.9399995803833
      },
      {
        "Date": "2010-02-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.329999923706055
      },
      {
        "Date": "2010-02-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.549999237060547
      },
      {
        "Date": "2010-02-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.65999984741211
      },
      {
        "Date": "2010-03-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.709999084472656
      },
      {
        "Date": "2010-03-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.459999084472656
      },
      {
        "Date": "2010-03-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.3700008392334
      },
      {
        "Date": "2010-03-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.399999618530273
      },
      {
        "Date": "2010-03-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.700000762939453
      },
      {
        "Date": "2010-03-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.739999771118164
      },
      {
        "Date": "2010-03-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.799999237060547
      },
      {
        "Date": "2010-03-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.110000610351562
      },
      {
        "Date": "2010-03-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.1200008392334
      },
      {
        "Date": "2010-03-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.850000381469727
      },
      {
        "Date": "2010-03-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.850000381469727
      },
      {
        "Date": "2010-03-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.030000686645508
      },
      {
        "Date": "2010-03-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.270000457763672
      },
      {
        "Date": "2010-03-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.079999923706055
      },
      {
        "Date": "2010-03-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.81999969482422
      },
      {
        "Date": "2010-03-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.959999084472656
      },
      {
        "Date": "2010-03-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.1299991607666
      },
      {
        "Date": "2010-03-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.56999969482422
      },
      {
        "Date": "2010-03-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.739999771118164
      },
      {
        "Date": "2010-03-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.899999618530273
      },
      {
        "Date": "2010-03-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.040000915527344
      },
      {
        "Date": "2010-03-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.760000228881836
      },
      {
        "Date": "2010-03-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.850000381469727
      },
      {
        "Date": "2010-04-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.040000915527344
      },
      {
        "Date": "2010-04-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.1299991607666
      },
      {
        "Date": "2010-04-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.489999771118164
      },
      {
        "Date": "2010-04-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.6200008392334
      },
      {
        "Date": "2010-04-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.649999618530273
      },
      {
        "Date": "2010-04-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.59000015258789
      },
      {
        "Date": "2010-04-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.65999984741211
      },
      {
        "Date": "2010-04-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.670000076293945
      },
      {
        "Date": "2010-04-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 19.399999618530273
      },
      {
        "Date": "2010-04-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 19.479999542236328
      },
      {
        "Date": "2010-04-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.40999984741211
      },
      {
        "Date": "2010-04-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.389999389648438
      },
      {
        "Date": "2010-04-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.610000610351562
      },
      {
        "Date": "2010-04-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.280000686645508
      },
      {
        "Date": "2010-04-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.540000915527344
      },
      {
        "Date": "2010-04-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.43000030517578
      },
      {
        "Date": "2010-04-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.049999237060547
      },
      {
        "Date": "2010-04-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.469999313354492
      },
      {
        "Date": "2010-04-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.780000686645508
      },
      {
        "Date": "2010-04-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.299999237060547
      },
      {
        "Date": "2010-04-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.829999923706055
      },
      {
        "Date": "2010-05-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 18.059999465942383
      },
      {
        "Date": "2010-05-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.559999465942383
      },
      {
        "Date": "2010-05-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.530000686645508
      },
      {
        "Date": "2010-05-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.280000686645508
      },
      {
        "Date": "2010-05-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.18000030517578
      },
      {
        "Date": "2010-05-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.299999237060547
      },
      {
        "Date": "2010-05-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.15999984741211
      },
      {
        "Date": "2010-05-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 17.06999969482422
      },
      {
        "Date": "2010-05-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.8700008392334
      },
      {
        "Date": "2010-05-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.34000015258789
      },
      {
        "Date": "2010-05-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.350000381469727
      },
      {
        "Date": "2010-05-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.949999809265137
      },
      {
        "Date": "2010-05-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.309999465942383
      },
      {
        "Date": "2010-05-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.300000190734863
      },
      {
        "Date": "2010-05-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.989999771118164
      },
      {
        "Date": "2010-05-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.399999618530273
      },
      {
        "Date": "2010-05-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.489999771118164
      },
      {
        "Date": "2010-05-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.470000267028809
      },
      {
        "Date": "2010-05-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 16.18000030517578
      },
      {
        "Date": "2010-05-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.739999771118164
      },
      {
        "Date": "2010-06-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.4399995803833
      },
      {
        "Date": "2010-06-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.890000343322754
      },
      {
        "Date": "2010-06-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.8100004196167
      },
      {
        "Date": "2010-06-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.350000381469727
      },
      {
        "Date": "2010-06-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.829999923706055
      },
      {
        "Date": "2010-06-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.329999923706055
      },
      {
        "Date": "2010-06-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.010000228881836
      },
      {
        "Date": "2010-06-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.460000038146973
      },
      {
        "Date": "2010-06-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.600000381469727
      },
      {
        "Date": "2010-06-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.40999984741211
      },
      {
        "Date": "2010-06-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.800000190734863
      },
      {
        "Date": "2010-06-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.869999885559082
      },
      {
        "Date": "2010-06-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.819999694824219
      },
      {
        "Date": "2010-06-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.819999694824219
      },
      {
        "Date": "2010-06-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.789999961853027
      },
      {
        "Date": "2010-06-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.579999923706055
      },
      {
        "Date": "2010-06-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.430000305175781
      },
      {
        "Date": "2010-06-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.020000457763672
      },
      {
        "Date": "2010-06-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.420000076293945
      },
      {
        "Date": "2010-06-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.239999771118164
      },
      {
        "Date": "2010-06-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.569999694824219
      },
      {
        "Date": "2010-06-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.369999885559082
      },
      {
        "Date": "2010-07-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.020000457763672
      },
      {
        "Date": "2010-07-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.84000015258789
      },
      {
        "Date": "2010-07-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.0600004196167
      },
      {
        "Date": "2010-07-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.710000038146973
      },
      {
        "Date": "2010-07-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.859999656677246
      },
      {
        "Date": "2010-07-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.109999656677246
      },
      {
        "Date": "2010-07-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.210000038146973
      },
      {
        "Date": "2010-07-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.670000076293945
      },
      {
        "Date": "2010-07-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.670000076293945
      },
      {
        "Date": "2010-07-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 15.390000343322754
      },
      {
        "Date": "2010-07-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.979999542236328
      },
      {
        "Date": "2010-07-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.609999656677246
      },
      {
        "Date": "2010-07-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.770000457763672
      },
      {
        "Date": "2010-07-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.359999656677246
      },
      {
        "Date": "2010-07-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.65999984741211
      },
      {
        "Date": "2010-07-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.739999771118164
      },
      {
        "Date": "2010-07-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.149999618530273
      },
      {
        "Date": "2010-07-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.1899995803833
      },
      {
        "Date": "2010-07-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.989999771118164
      },
      {
        "Date": "2010-07-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.029999732971191
      },
      {
        "Date": "2010-07-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.039999961853027
      },
      {
        "Date": "2010-08-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.4399995803833
      },
      {
        "Date": "2010-08-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.34000015258789
      },
      {
        "Date": "2010-08-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.1899995803833
      },
      {
        "Date": "2010-08-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 14.020000457763672
      },
      {
        "Date": "2010-08-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.960000038146973
      },
      {
        "Date": "2010-08-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.90999984741211
      },
      {
        "Date": "2010-08-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.630000114440918
      },
      {
        "Date": "2010-08-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.1899995803833
      },
      {
        "Date": "2010-08-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.0600004196167
      },
      {
        "Date": "2010-08-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.229999542236328
      },
      {
        "Date": "2010-08-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.1899995803833
      },
      {
        "Date": "2010-08-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.210000038146973
      },
      {
        "Date": "2010-08-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.319999694824219
      },
      {
        "Date": "2010-08-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.020000457763672
      },
      {
        "Date": "2010-08-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.869999885559082
      },
      {
        "Date": "2010-08-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.869999885559082
      },
      {
        "Date": "2010-08-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.640000343322754
      },
      {
        "Date": "2010-08-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.65999984741211
      },
      {
        "Date": "2010-08-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.470000267028809
      },
      {
        "Date": "2010-08-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.640000343322754
      },
      {
        "Date": "2010-08-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.319999694824219
      },
      {
        "Date": "2010-08-31T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.460000038146973
      },
      {
        "Date": "2010-09-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.210000038146973
      },
      {
        "Date": "2010-09-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.279999732971191
      },
      {"Date": "2010-09-03T00:00:00", "Bank": "BAC", "Stock Price": 13.5},
      {
        "Date": "2010-09-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.210000038146973
      },
      {
        "Date": "2010-09-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.369999885559082
      },
      {"Date": "2010-09-09T00:00:00", "Bank": "BAC", "Stock Price": 13.5},
      {
        "Date": "2010-09-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.550000190734863
      },
      {
        "Date": "2010-09-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.949999809265137
      },
      {
        "Date": "2010-09-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.680000305175781
      },
      {
        "Date": "2010-09-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.710000038146973
      },
      {
        "Date": "2010-09-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.550000190734863
      },
      {
        "Date": "2010-09-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.399999618530273
      },
      {
        "Date": "2010-09-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.739999771118164
      },
      {
        "Date": "2010-09-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.649999618530273
      },
      {
        "Date": "2010-09-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.420000076293945
      },
      {
        "Date": "2010-09-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.170000076293945
      },
      {
        "Date": "2010-09-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.600000381469727
      },
      {
        "Date": "2010-09-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.239999771118164
      },
      {
        "Date": "2010-09-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.270000457763672
      },
      {
        "Date": "2010-09-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.109999656677246
      },
      {
        "Date": "2010-09-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.100000381469727
      },
      {
        "Date": "2010-10-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.300000190734863
      },
      {
        "Date": "2010-10-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.149999618530273
      },
      {
        "Date": "2010-10-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.5600004196167
      },
      {
        "Date": "2010-10-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.390000343322754
      },
      {
        "Date": "2010-10-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.3100004196167
      },
      {
        "Date": "2010-10-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.180000305175781
      },
      {
        "Date": "2010-10-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.149999618530273
      },
      {
        "Date": "2010-10-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.520000457763672
      },
      {
        "Date": "2010-10-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.289999961853027
      },
      {
        "Date": "2010-10-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.600000381469727
      },
      {
        "Date": "2010-10-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.979999542236328
      },
      {
        "Date": "2010-10-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.34000015258789
      },
      {
        "Date": "2010-10-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.800000190734863
      },
      {"Date": "2010-10-20T00:00:00", "Bank": "BAC", "Stock Price": 11.75},
      {
        "Date": "2010-10-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.359999656677246
      },
      {
        "Date": "2010-10-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.4399995803833
      },
      {
        "Date": "2010-10-25T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.15999984741211
      },
      {
        "Date": "2010-10-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.300000190734863
      },
      {
        "Date": "2010-10-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.539999961853027
      },
      {
        "Date": "2010-10-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.529999732971191
      },
      {
        "Date": "2010-10-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.449999809265137
      },
      {"Date": "2010-11-01T00:00:00", "Bank": "BAC", "Stock Price": 11.5},
      {
        "Date": "2010-11-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.399999618530273
      },
      {
        "Date": "2010-11-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.520000457763672
      },
      {
        "Date": "2010-11-04T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.130000114440918
      },
      {
        "Date": "2010-11-05T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.359999656677246
      },
      {
        "Date": "2010-11-08T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.600000381469727
      },
      {
        "Date": "2010-11-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.270000457763672
      },
      {
        "Date": "2010-11-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.569999694824219
      },
      {
        "Date": "2010-11-11T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.369999885559082
      },
      {
        "Date": "2010-11-12T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.119999885559082
      },
      {
        "Date": "2010-11-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.100000381469727
      },
      {
        "Date": "2010-11-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.9399995803833
      },
      {
        "Date": "2010-11-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.619999885559082
      },
      {
        "Date": "2010-11-18T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.699999809265137
      },
      {
        "Date": "2010-11-19T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.65999984741211
      },
      {
        "Date": "2010-11-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.300000190734863
      },
      {
        "Date": "2010-11-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.09000015258789
      },
      {
        "Date": "2010-11-24T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.279999732971191
      },
      {
        "Date": "2010-11-26T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.119999885559082
      },
      {
        "Date": "2010-11-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.3100004196167
      },
      {
        "Date": "2010-11-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 10.949999809265137
      },
      {
        "Date": "2010-12-01T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.289999961853027
      },
      {
        "Date": "2010-12-02T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.680000305175781
      },
      {
        "Date": "2010-12-03T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.859999656677246
      },
      {
        "Date": "2010-12-06T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.640000343322754
      },
      {
        "Date": "2010-12-07T00:00:00",
        "Bank": "BAC",
        "Stock Price": 11.569999694824219
      },
      {"Date": "2010-12-08T00:00:00", "Bank": "BAC", "Stock Price": 12},
      {
        "Date": "2010-12-09T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.649999618530273
      },
      {
        "Date": "2010-12-10T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.800000190734863
      },
      {
        "Date": "2010-12-13T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.539999961853027
      },
      {
        "Date": "2010-12-14T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.399999618530273
      },
      {
        "Date": "2010-12-15T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.289999961853027
      },
      {
        "Date": "2010-12-16T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.520000457763672
      },
      {
        "Date": "2010-12-17T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.569999694824219
      },
      {
        "Date": "2010-12-20T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.619999885559082
      },
      {
        "Date": "2010-12-21T00:00:00",
        "Bank": "BAC",
        "Stock Price": 12.979999542236328
      },
      {
        "Date": "2010-12-22T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.380000114440918
      },
      {
        "Date": "2010-12-23T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.0600004196167
      },
      {
        "Date": "2010-12-27T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.270000457763672
      },
      {
        "Date": "2010-12-28T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.34000015258789
      },
      {
        "Date": "2010-12-29T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.3100004196167
      },
      {
        "Date": "2010-12-30T00:00:00",
        "Bank": "BAC",
        "Stock Price": 13.279999732971191
      },
      {"Date": "2007-01-03T00:00:00", "Bank": "C", "Stock Price": 552.5},
      {
        "Date": "2007-01-04T00:00:00",
        "Bank": "C",
        "Stock Price": 550.5999755859375
      },
      {
        "Date": "2007-01-05T00:00:00",
        "Bank": "C",
        "Stock Price": 547.7000122070312
      },
      {"Date": "2007-01-08T00:00:00", "Bank": "C", "Stock Price": 550.5},
      {
        "Date": "2007-01-09T00:00:00",
        "Bank": "C",
        "Stock Price": 545.7000122070312
      },
      {
        "Date": "2007-01-10T00:00:00",
        "Bank": "C",
        "Stock Price": 541.2999877929688
      },
      {
        "Date": "2007-01-11T00:00:00",
        "Bank": "C",
        "Stock Price": 541.7000122070312
      },
      {
        "Date": "2007-01-12T00:00:00",
        "Bank": "C",
        "Stock Price": 543.7999877929688
      },
      {
        "Date": "2007-01-16T00:00:00",
        "Bank": "C",
        "Stock Price": 547.7000122070312
      },
      {
        "Date": "2007-01-17T00:00:00",
        "Bank": "C",
        "Stock Price": 543.9000244140625
      },
      {
        "Date": "2007-01-18T00:00:00",
        "Bank": "C",
        "Stock Price": 543.9000244140625
      },
      {"Date": "2007-01-19T00:00:00", "Bank": "C", "Stock Price": 545},
      {
        "Date": "2007-01-22T00:00:00",
        "Bank": "C",
        "Stock Price": 546.7999877929688
      },
      {
        "Date": "2007-01-23T00:00:00",
        "Bank": "C",
        "Stock Price": 544.9000244140625
      },
      {
        "Date": "2007-01-24T00:00:00",
        "Bank": "C",
        "Stock Price": 548.2999877929688
      },
      {
        "Date": "2007-01-25T00:00:00",
        "Bank": "C",
        "Stock Price": 539.2999877929688
      },
      {
        "Date": "2007-01-26T00:00:00",
        "Bank": "C",
        "Stock Price": 546.7000122070312
      },
      {
        "Date": "2007-01-29T00:00:00",
        "Bank": "C",
        "Stock Price": 540.5999755859375
      },
      {
        "Date": "2007-01-30T00:00:00",
        "Bank": "C",
        "Stock Price": 542.7000122070312
      },
      {
        "Date": "2007-01-31T00:00:00",
        "Bank": "C",
        "Stock Price": 551.2999877929688
      },
      {
        "Date": "2007-02-01T00:00:00",
        "Bank": "C",
        "Stock Price": 547.2999877929688
      },
      {
        "Date": "2007-02-02T00:00:00",
        "Bank": "C",
        "Stock Price": 546.5999755859375
      },
      {"Date": "2007-02-05T00:00:00", "Bank": "C", "Stock Price": 547.5},
      {"Date": "2007-02-06T00:00:00", "Bank": "C", "Stock Price": 549.5},
      {"Date": "2007-02-07T00:00:00", "Bank": "C", "Stock Price": 549.5},
      {
        "Date": "2007-02-08T00:00:00",
        "Bank": "C",
        "Stock Price": 544.4000244140625
      },
      {"Date": "2007-02-09T00:00:00", "Bank": "C", "Stock Price": 534},
      {
        "Date": "2007-02-12T00:00:00",
        "Bank": "C",
        "Stock Price": 534.2999877929688
      },
      {
        "Date": "2007-02-13T00:00:00",
        "Bank": "C",
        "Stock Price": 537.0999755859375
      },
      {
        "Date": "2007-02-14T00:00:00",
        "Bank": "C",
        "Stock Price": 541.7999877929688
      },
      {
        "Date": "2007-02-15T00:00:00",
        "Bank": "C",
        "Stock Price": 542.0999755859375
      },
      {"Date": "2007-02-16T00:00:00", "Bank": "C", "Stock Price": 541},
      {
        "Date": "2007-02-20T00:00:00",
        "Bank": "C",
        "Stock Price": 541.9000244140625
      },
      {"Date": "2007-02-21T00:00:00", "Bank": "C", "Stock Price": 537.5},
      {
        "Date": "2007-02-22T00:00:00",
        "Bank": "C",
        "Stock Price": 535.9000244140625
      },
      {
        "Date": "2007-02-23T00:00:00",
        "Bank": "C",
        "Stock Price": 537.7000122070312
      },
      {
        "Date": "2007-02-26T00:00:00",
        "Bank": "C",
        "Stock Price": 526.7999877929688
      },
      {"Date": "2007-02-27T00:00:00", "Bank": "C", "Stock Price": 506},
      {
        "Date": "2007-02-28T00:00:00",
        "Bank": "C",
        "Stock Price": 503.70001220703125
      },
      {
        "Date": "2007-03-01T00:00:00",
        "Bank": "C",
        "Stock Price": 510.79998779296875
      },
      {
        "Date": "2007-03-02T00:00:00",
        "Bank": "C",
        "Stock Price": 499.70001220703125
      },
      {"Date": "2007-03-05T00:00:00", "Bank": "C", "Stock Price": 492.5},
      {
        "Date": "2007-03-06T00:00:00",
        "Bank": "C",
        "Stock Price": 505.79998779296875
      },
      {
        "Date": "2007-03-07T00:00:00",
        "Bank": "C",
        "Stock Price": 502.20001220703125
      },
      {"Date": "2007-03-08T00:00:00", "Bank": "C", "Stock Price": 505},
      {
        "Date": "2007-03-09T00:00:00",
        "Bank": "C",
        "Stock Price": 503.29998779296875
      },
      {
        "Date": "2007-03-12T00:00:00",
        "Bank": "C",
        "Stock Price": 503.6000061035156
      },
      {"Date": "2007-03-13T00:00:00", "Bank": "C", "Stock Price": 487.5},
      {
        "Date": "2007-03-14T00:00:00",
        "Bank": "C",
        "Stock Price": 490.79998779296875
      },
      {
        "Date": "2007-03-15T00:00:00",
        "Bank": "C",
        "Stock Price": 501.29998779296875
      },
      {
        "Date": "2007-03-16T00:00:00",
        "Bank": "C",
        "Stock Price": 495.29998779296875
      },
      {
        "Date": "2007-03-19T00:00:00",
        "Bank": "C",
        "Stock Price": 500.6000061035156
      },
      {
        "Date": "2007-03-20T00:00:00",
        "Bank": "C",
        "Stock Price": 506.3999938964844
      },
      {
        "Date": "2007-03-21T00:00:00",
        "Bank": "C",
        "Stock Price": 520.2999877929688
      },
      {
        "Date": "2007-03-22T00:00:00",
        "Bank": "C",
        "Stock Price": 518.4000244140625
      },
      {
        "Date": "2007-03-23T00:00:00",
        "Bank": "C",
        "Stock Price": 517.2000122070312
      },
      {
        "Date": "2007-03-26T00:00:00",
        "Bank": "C",
        "Stock Price": 515.4000244140625
      },
      {
        "Date": "2007-03-27T00:00:00",
        "Bank": "C",
        "Stock Price": 510.6000061035156
      },
      {
        "Date": "2007-03-28T00:00:00",
        "Bank": "C",
        "Stock Price": 509.6000061035156
      },
      {"Date": "2007-03-29T00:00:00", "Bank": "C", "Stock Price": 514},
      {
        "Date": "2007-03-30T00:00:00",
        "Bank": "C",
        "Stock Price": 513.4000244140625
      },
      {"Date": "2007-04-02T00:00:00", "Bank": "C", "Stock Price": 510.5},
      {
        "Date": "2007-04-03T00:00:00",
        "Bank": "C",
        "Stock Price": 514.0999755859375
      },
      {
        "Date": "2007-04-04T00:00:00",
        "Bank": "C",
        "Stock Price": 513.5999755859375
      },
      {
        "Date": "2007-04-05T00:00:00",
        "Bank": "C",
        "Stock Price": 515.7000122070312
      },
      {
        "Date": "2007-04-09T00:00:00",
        "Bank": "C",
        "Stock Price": 515.7999877929688
      },
      {"Date": "2007-04-10T00:00:00", "Bank": "C", "Stock Price": 524},
      {"Date": "2007-04-11T00:00:00", "Bank": "C", "Stock Price": 518},
      {"Date": "2007-04-12T00:00:00", "Bank": "C", "Stock Price": 516.5},
      {"Date": "2007-04-13T00:00:00", "Bank": "C", "Stock Price": 516},
      {
        "Date": "2007-04-16T00:00:00",
        "Bank": "C",
        "Stock Price": 529.2999877929688
      },
      {
        "Date": "2007-04-17T00:00:00",
        "Bank": "C",
        "Stock Price": 525.2999877929688
      },
      {
        "Date": "2007-04-18T00:00:00",
        "Bank": "C",
        "Stock Price": 529.9000244140625
      },
      {
        "Date": "2007-04-19T00:00:00",
        "Bank": "C",
        "Stock Price": 530.9000244140625
      },
      {
        "Date": "2007-04-20T00:00:00",
        "Bank": "C",
        "Stock Price": 534.2000122070312
      },
      {
        "Date": "2007-04-23T00:00:00",
        "Bank": "C",
        "Stock Price": 531.0999755859375
      },
      {
        "Date": "2007-04-24T00:00:00",
        "Bank": "C",
        "Stock Price": 528.0999755859375
      },
      {"Date": "2007-04-25T00:00:00", "Bank": "C", "Stock Price": 538},
      {
        "Date": "2007-04-26T00:00:00",
        "Bank": "C",
        "Stock Price": 535.5999755859375
      },
      {
        "Date": "2007-04-27T00:00:00",
        "Bank": "C",
        "Stock Price": 533.7000122070312
      },
      {
        "Date": "2007-04-30T00:00:00",
        "Bank": "C",
        "Stock Price": 536.2000122070312
      },
      {"Date": "2007-05-01T00:00:00", "Bank": "C", "Stock Price": 542},
      {"Date": "2007-05-02T00:00:00", "Bank": "C", "Stock Price": 543},
      {"Date": "2007-05-03T00:00:00", "Bank": "C", "Stock Price": 539.5},
      {
        "Date": "2007-05-04T00:00:00",
        "Bank": "C",
        "Stock Price": 540.9000244140625
      },
      {
        "Date": "2007-05-07T00:00:00",
        "Bank": "C",
        "Stock Price": 538.7999877929688
      },
      {
        "Date": "2007-05-08T00:00:00",
        "Bank": "C",
        "Stock Price": 537.2000122070312
      },
      {
        "Date": "2007-05-09T00:00:00",
        "Bank": "C",
        "Stock Price": 541.2000122070312
      },
      {"Date": "2007-05-10T00:00:00", "Bank": "C", "Stock Price": 532},
      {
        "Date": "2007-05-11T00:00:00",
        "Bank": "C",
        "Stock Price": 531.0999755859375
      },
      {
        "Date": "2007-05-14T00:00:00",
        "Bank": "C",
        "Stock Price": 528.5999755859375
      },
      {
        "Date": "2007-05-15T00:00:00",
        "Bank": "C",
        "Stock Price": 527.9000244140625
      },
      {
        "Date": "2007-05-16T00:00:00",
        "Bank": "C",
        "Stock Price": 549.0999755859375
      },
      {"Date": "2007-05-17T00:00:00", "Bank": "C", "Stock Price": 548},
      {"Date": "2007-05-18T00:00:00", "Bank": "C", "Stock Price": 550},
      {
        "Date": "2007-05-21T00:00:00",
        "Bank": "C",
        "Stock Price": 548.4000244140625
      },
      {
        "Date": "2007-05-22T00:00:00",
        "Bank": "C",
        "Stock Price": 550.7999877929688
      },
      {
        "Date": "2007-05-23T00:00:00",
        "Bank": "C",
        "Stock Price": 550.0999755859375
      },
      {
        "Date": "2007-05-24T00:00:00",
        "Bank": "C",
        "Stock Price": 549.2999877929688
      },
      {
        "Date": "2007-05-25T00:00:00",
        "Bank": "C",
        "Stock Price": 551.2000122070312
      },
      {
        "Date": "2007-05-29T00:00:00",
        "Bank": "C",
        "Stock Price": 549.0999755859375
      },
      {"Date": "2007-05-30T00:00:00", "Bank": "C", "Stock Price": 552},
      {
        "Date": "2007-05-31T00:00:00",
        "Bank": "C",
        "Stock Price": 544.9000244140625
      },
      {
        "Date": "2007-06-01T00:00:00",
        "Bank": "C",
        "Stock Price": 545.0999755859375
      },
      {"Date": "2007-06-04T00:00:00", "Bank": "C", "Stock Price": 541.5},
      {"Date": "2007-06-05T00:00:00", "Bank": "C", "Stock Price": 539},
      {
        "Date": "2007-06-06T00:00:00",
        "Bank": "C",
        "Stock Price": 533.2999877929688
      },
      {
        "Date": "2007-06-07T00:00:00",
        "Bank": "C",
        "Stock Price": 525.2000122070312
      },
      {
        "Date": "2007-06-08T00:00:00",
        "Bank": "C",
        "Stock Price": 533.2999877929688
      },
      {
        "Date": "2007-06-11T00:00:00",
        "Bank": "C",
        "Stock Price": 534.7000122070312
      },
      {"Date": "2007-06-12T00:00:00", "Bank": "C", "Stock Price": 526},
      {
        "Date": "2007-06-13T00:00:00",
        "Bank": "C",
        "Stock Price": 536.7999877929688
      },
      {
        "Date": "2007-06-14T00:00:00",
        "Bank": "C",
        "Stock Price": 536.7000122070312
      },
      {
        "Date": "2007-06-15T00:00:00",
        "Bank": "C",
        "Stock Price": 539.7999877929688
      },
      {
        "Date": "2007-06-18T00:00:00",
        "Bank": "C",
        "Stock Price": 539.5999755859375
      },
      {
        "Date": "2007-06-19T00:00:00",
        "Bank": "C",
        "Stock Price": 542.5999755859375
      },
      {
        "Date": "2007-06-20T00:00:00",
        "Bank": "C",
        "Stock Price": 534.4000244140625
      },
      {
        "Date": "2007-06-21T00:00:00",
        "Bank": "C",
        "Stock Price": 536.5999755859375
      },
      {
        "Date": "2007-06-22T00:00:00",
        "Bank": "C",
        "Stock Price": 524.0999755859375
      },
      {
        "Date": "2007-06-25T00:00:00",
        "Bank": "C",
        "Stock Price": 516.9000244140625
      },
      {"Date": "2007-06-26T00:00:00", "Bank": "C", "Stock Price": 511.5},
      {
        "Date": "2007-06-27T00:00:00",
        "Bank": "C",
        "Stock Price": 518.0999755859375
      },
      {
        "Date": "2007-06-28T00:00:00",
        "Bank": "C",
        "Stock Price": 518.0999755859375
      },
      {
        "Date": "2007-06-29T00:00:00",
        "Bank": "C",
        "Stock Price": 512.9000244140625
      },
      {
        "Date": "2007-07-02T00:00:00",
        "Bank": "C",
        "Stock Price": 516.4000244140625
      },
      {
        "Date": "2007-07-03T00:00:00",
        "Bank": "C",
        "Stock Price": 518.5999755859375
      },
      {"Date": "2007-07-05T00:00:00", "Bank": "C", "Stock Price": 515},
      {"Date": "2007-07-06T00:00:00", "Bank": "C", "Stock Price": 517},
      {"Date": "2007-07-09T00:00:00", "Bank": "C", "Stock Price": 516},
      {"Date": "2007-07-10T00:00:00", "Bank": "C", "Stock Price": 510},
      {
        "Date": "2007-07-11T00:00:00",
        "Bank": "C",
        "Stock Price": 514.0999755859375
      },
      {
        "Date": "2007-07-12T00:00:00",
        "Bank": "C",
        "Stock Price": 528.4000244140625
      },
      {
        "Date": "2007-07-13T00:00:00",
        "Bank": "C",
        "Stock Price": 525.2000122070312
      },
      {
        "Date": "2007-07-16T00:00:00",
        "Bank": "C",
        "Stock Price": 521.9000244140625
      },
      {
        "Date": "2007-07-17T00:00:00",
        "Bank": "C",
        "Stock Price": 524.5999755859375
      },
      {"Date": "2007-07-18T00:00:00", "Bank": "C", "Stock Price": 516},
      {
        "Date": "2007-07-19T00:00:00",
        "Bank": "C",
        "Stock Price": 511.29998779296875
      },
      {
        "Date": "2007-07-20T00:00:00",
        "Bank": "C",
        "Stock Price": 507.29998779296875
      },
      {
        "Date": "2007-07-23T00:00:00",
        "Bank": "C",
        "Stock Price": 508.6000061035156
      },
      {
        "Date": "2007-07-24T00:00:00",
        "Bank": "C",
        "Stock Price": 493.1000061035156
      },
      {
        "Date": "2007-07-25T00:00:00",
        "Bank": "C",
        "Stock Price": 492.1000061035156
      },
      {
        "Date": "2007-07-26T00:00:00",
        "Bank": "C",
        "Stock Price": 478.1000061035156
      },
      {
        "Date": "2007-07-27T00:00:00",
        "Bank": "C",
        "Stock Price": 469.70001220703125
      },
      {
        "Date": "2007-07-30T00:00:00",
        "Bank": "C",
        "Stock Price": 471.8999938964844
      },
      {
        "Date": "2007-07-31T00:00:00",
        "Bank": "C",
        "Stock Price": 465.70001220703125
      },
      {"Date": "2007-08-01T00:00:00", "Bank": "C", "Stock Price": 468.5},
      {
        "Date": "2007-08-02T00:00:00",
        "Bank": "C",
        "Stock Price": 472.3999938964844
      },
      {
        "Date": "2007-08-03T00:00:00",
        "Bank": "C",
        "Stock Price": 457.20001220703125
      },
      {"Date": "2007-08-06T00:00:00", "Bank": "C", "Stock Price": 483.5},
      {
        "Date": "2007-08-07T00:00:00",
        "Bank": "C",
        "Stock Price": 485.8999938964844
      },
      {
        "Date": "2007-08-08T00:00:00",
        "Bank": "C",
        "Stock Price": 494.8999938964844
      },
      {"Date": "2007-08-09T00:00:00", "Bank": "C", "Stock Price": 469},
      {"Date": "2007-08-10T00:00:00", "Bank": "C", "Stock Price": 470},
      {
        "Date": "2007-08-13T00:00:00",
        "Bank": "C",
        "Stock Price": 465.3999938964844
      },
      {
        "Date": "2007-08-14T00:00:00",
        "Bank": "C",
        "Stock Price": 456.6000061035156
      },
      {
        "Date": "2007-08-15T00:00:00",
        "Bank": "C",
        "Stock Price": 456.1000061035156
      },
      {"Date": "2007-08-16T00:00:00", "Bank": "C", "Stock Price": 475.5},
      {
        "Date": "2007-08-17T00:00:00",
        "Bank": "C",
        "Stock Price": 488.1000061035156
      },
      {
        "Date": "2007-08-20T00:00:00",
        "Bank": "C",
        "Stock Price": 483.8999938964844
      },
      {
        "Date": "2007-08-21T00:00:00",
        "Bank": "C",
        "Stock Price": 480.6000061035156
      },
      {
        "Date": "2007-08-22T00:00:00",
        "Bank": "C",
        "Stock Price": 484.29998779296875
      },
      {"Date": "2007-08-23T00:00:00", "Bank": "C", "Stock Price": 483.5},
      {"Date": "2007-08-24T00:00:00", "Bank": "C", "Stock Price": 485},
      {
        "Date": "2007-08-27T00:00:00",
        "Bank": "C",
        "Stock Price": 477.8999938964844
      },
      {
        "Date": "2007-08-28T00:00:00",
        "Bank": "C",
        "Stock Price": 461.3999938964844
      },
      {"Date": "2007-08-29T00:00:00", "Bank": "C", "Stock Price": 469.5},
      {
        "Date": "2007-08-30T00:00:00",
        "Bank": "C",
        "Stock Price": 462.29998779296875
      },
      {
        "Date": "2007-08-31T00:00:00",
        "Bank": "C",
        "Stock Price": 468.79998779296875
      },
      {
        "Date": "2007-09-04T00:00:00",
        "Bank": "C",
        "Stock Price": 472.1000061035156
      },
      {"Date": "2007-09-05T00:00:00", "Bank": "C", "Stock Price": 460},
      {
        "Date": "2007-09-06T00:00:00",
        "Bank": "C",
        "Stock Price": 456.6000061035156
      },
      {
        "Date": "2007-09-07T00:00:00",
        "Bank": "C",
        "Stock Price": 454.79998779296875
      },
      {"Date": "2007-09-10T00:00:00", "Bank": "C", "Stock Price": 453},
      {
        "Date": "2007-09-11T00:00:00",
        "Bank": "C",
        "Stock Price": 460.1000061035156
      },
      {
        "Date": "2007-09-12T00:00:00",
        "Bank": "C",
        "Stock Price": 457.6000061035156
      },
      {
        "Date": "2007-09-13T00:00:00",
        "Bank": "C",
        "Stock Price": 463.6000061035156
      },
      {
        "Date": "2007-09-14T00:00:00",
        "Bank": "C",
        "Stock Price": 466.3999938964844
      },
      {
        "Date": "2007-09-17T00:00:00",
        "Bank": "C",
        "Stock Price": 460.29998779296875
      },
      {
        "Date": "2007-09-18T00:00:00",
        "Bank": "C",
        "Stock Price": 483.70001220703125
      },
      {
        "Date": "2007-09-19T00:00:00",
        "Bank": "C",
        "Stock Price": 482.70001220703125
      },
      {"Date": "2007-09-20T00:00:00", "Bank": "C", "Stock Price": 472},
      {
        "Date": "2007-09-21T00:00:00",
        "Bank": "C",
        "Stock Price": 475.1000061035156
      },
      {
        "Date": "2007-09-24T00:00:00",
        "Bank": "C",
        "Stock Price": 465.8999938964844
      },
      {
        "Date": "2007-09-25T00:00:00",
        "Bank": "C",
        "Stock Price": 463.1000061035156
      },
      {"Date": "2007-09-26T00:00:00", "Bank": "C", "Stock Price": 465.5},
      {
        "Date": "2007-09-27T00:00:00",
        "Bank": "C",
        "Stock Price": 468.79998779296875
      },
      {
        "Date": "2007-09-28T00:00:00",
        "Bank": "C",
        "Stock Price": 466.70001220703125
      },
      {
        "Date": "2007-10-01T00:00:00",
        "Bank": "C",
        "Stock Price": 477.20001220703125
      },
      {
        "Date": "2007-10-02T00:00:00",
        "Bank": "C",
        "Stock Price": 478.6000061035156
      },
      {
        "Date": "2007-10-03T00:00:00",
        "Bank": "C",
        "Stock Price": 478.8999938964844
      },
      {
        "Date": "2007-10-04T00:00:00",
        "Bank": "C",
        "Stock Price": 476.29998779296875
      },
      {"Date": "2007-10-05T00:00:00", "Bank": "C", "Stock Price": 483},
      {"Date": "2007-10-08T00:00:00", "Bank": "C", "Stock Price": 478},
      {
        "Date": "2007-10-09T00:00:00",
        "Bank": "C",
        "Stock Price": 476.20001220703125
      },
      {
        "Date": "2007-10-10T00:00:00",
        "Bank": "C",
        "Stock Price": 471.3999938964844
      },
      {
        "Date": "2007-10-11T00:00:00",
        "Bank": "C",
        "Stock Price": 483.20001220703125
      },
      {
        "Date": "2007-10-12T00:00:00",
        "Bank": "C",
        "Stock Price": 478.70001220703125
      },
      {
        "Date": "2007-10-15T00:00:00",
        "Bank": "C",
        "Stock Price": 462.3999938964844
      },
      {
        "Date": "2007-10-16T00:00:00",
        "Bank": "C",
        "Stock Price": 447.8999938964844
      },
      {
        "Date": "2007-10-17T00:00:00",
        "Bank": "C",
        "Stock Price": 446.6000061035156
      },
      {
        "Date": "2007-10-18T00:00:00",
        "Bank": "C",
        "Stock Price": 438.29998779296875
      },
      {
        "Date": "2007-10-19T00:00:00",
        "Bank": "C",
        "Stock Price": 423.6000061035156
      },
      {
        "Date": "2007-10-22T00:00:00",
        "Bank": "C",
        "Stock Price": 426.1000061035156
      },
      {
        "Date": "2007-10-23T00:00:00",
        "Bank": "C",
        "Stock Price": 424.3999938964844
      },
      {
        "Date": "2007-10-24T00:00:00",
        "Bank": "C",
        "Stock Price": 418.20001220703125
      },
      {
        "Date": "2007-10-25T00:00:00",
        "Bank": "C",
        "Stock Price": 412.29998779296875
      },
      {
        "Date": "2007-10-26T00:00:00",
        "Bank": "C",
        "Stock Price": 426.29998779296875
      },
      {
        "Date": "2007-10-29T00:00:00",
        "Bank": "C",
        "Stock Price": 426.8999938964844
      },
      {
        "Date": "2007-10-30T00:00:00",
        "Bank": "C",
        "Stock Price": 421.1000061035156
      },
      {"Date": "2007-10-31T00:00:00", "Bank": "C", "Stock Price": 419},
      {
        "Date": "2007-11-01T00:00:00",
        "Bank": "C",
        "Stock Price": 385.1000061035156
      },
      {
        "Date": "2007-11-02T00:00:00",
        "Bank": "C",
        "Stock Price": 377.29998779296875
      },
      {"Date": "2007-11-05T00:00:00", "Bank": "C", "Stock Price": 359},
      {
        "Date": "2007-11-06T00:00:00",
        "Bank": "C",
        "Stock Price": 350.79998779296875
      },
      {
        "Date": "2007-11-07T00:00:00",
        "Bank": "C",
        "Stock Price": 334.1000061035156
      },
      {"Date": "2007-11-08T00:00:00", "Bank": "C", "Stock Price": 329},
      {"Date": "2007-11-09T00:00:00", "Bank": "C", "Stock Price": 331},
      {
        "Date": "2007-11-12T00:00:00",
        "Bank": "C",
        "Stock Price": 335.70001220703125
      },
      {"Date": "2007-11-13T00:00:00", "Bank": "C", "Stock Price": 359},
      {
        "Date": "2007-11-14T00:00:00",
        "Bank": "C",
        "Stock Price": 360.3999938964844
      },
      {
        "Date": "2007-11-15T00:00:00",
        "Bank": "C",
        "Stock Price": 345.79998779296875
      },
      {"Date": "2007-11-16T00:00:00", "Bank": "C", "Stock Price": 340},
      {"Date": "2007-11-19T00:00:00", "Bank": "C", "Stock Price": 320},
      {"Date": "2007-11-20T00:00:00", "Bank": "C", "Stock Price": 314},
      {
        "Date": "2007-11-21T00:00:00",
        "Bank": "C",
        "Stock Price": 307.29998779296875
      },
      {"Date": "2007-11-23T00:00:00", "Bank": "C", "Stock Price": 317},
      {"Date": "2007-11-26T00:00:00", "Bank": "C", "Stock Price": 307},
      {
        "Date": "2007-11-27T00:00:00",
        "Bank": "C",
        "Stock Price": 303.20001220703125
      },
      {
        "Date": "2007-11-28T00:00:00",
        "Bank": "C",
        "Stock Price": 322.8999938964844
      },
      {
        "Date": "2007-11-29T00:00:00",
        "Bank": "C",
        "Stock Price": 322.8999938964844
      },
      {"Date": "2007-11-30T00:00:00", "Bank": "C", "Stock Price": 333},
      {
        "Date": "2007-12-03T00:00:00",
        "Bank": "C",
        "Stock Price": 330.6000061035156
      },
      {"Date": "2007-12-04T00:00:00", "Bank": "C", "Stock Price": 325.5},
      {
        "Date": "2007-12-05T00:00:00",
        "Bank": "C",
        "Stock Price": 336.8999938964844
      },
      {"Date": "2007-12-06T00:00:00", "Bank": "C", "Stock Price": 343.5},
      {
        "Date": "2007-12-07T00:00:00",
        "Bank": "C",
        "Stock Price": 343.1000061035156
      },
      {
        "Date": "2007-12-10T00:00:00",
        "Bank": "C",
        "Stock Price": 347.70001220703125
      },
      {
        "Date": "2007-12-11T00:00:00",
        "Bank": "C",
        "Stock Price": 332.29998779296875
      },
      {
        "Date": "2007-12-12T00:00:00",
        "Bank": "C",
        "Stock Price": 314.70001220703125
      },
      {
        "Date": "2007-12-13T00:00:00",
        "Bank": "C",
        "Stock Price": 310.1000061035156
      },
      {"Date": "2007-12-14T00:00:00", "Bank": "C", "Stock Price": 307},
      {
        "Date": "2007-12-17T00:00:00",
        "Bank": "C",
        "Stock Price": 307.70001220703125
      },
      {
        "Date": "2007-12-18T00:00:00",
        "Bank": "C",
        "Stock Price": 303.79998779296875
      },
      {
        "Date": "2007-12-19T00:00:00",
        "Bank": "C",
        "Stock Price": 302.1000061035156
      },
      {
        "Date": "2007-12-20T00:00:00",
        "Bank": "C",
        "Stock Price": 298.8999938964844
      },
      {
        "Date": "2007-12-21T00:00:00",
        "Bank": "C",
        "Stock Price": 302.3999938964844
      },
      {
        "Date": "2007-12-24T00:00:00",
        "Bank": "C",
        "Stock Price": 309.79998779296875
      },
      {"Date": "2007-12-26T00:00:00", "Bank": "C", "Stock Price": 304.5},
      {
        "Date": "2007-12-27T00:00:00",
        "Bank": "C",
        "Stock Price": 295.6000061035156
      },
      {
        "Date": "2007-12-28T00:00:00",
        "Bank": "C",
        "Stock Price": 292.8999938964844
      },
      {
        "Date": "2007-12-31T00:00:00",
        "Bank": "C",
        "Stock Price": 294.3999938964844
      },
      {
        "Date": "2008-01-02T00:00:00",
        "Bank": "C",
        "Stock Price": 289.20001220703125
      },
      {
        "Date": "2008-01-03T00:00:00",
        "Bank": "C",
        "Stock Price": 289.29998779296875
      },
      {
        "Date": "2008-01-04T00:00:00",
        "Bank": "C",
        "Stock Price": 282.3999938964844
      },
      {
        "Date": "2008-01-07T00:00:00",
        "Bank": "C",
        "Stock Price": 282.6000061035156
      },
      {
        "Date": "2008-01-08T00:00:00",
        "Bank": "C",
        "Stock Price": 271.3999938964844
      },
      {
        "Date": "2008-01-09T00:00:00",
        "Bank": "C",
        "Stock Price": 274.8999938964844
      },
      {
        "Date": "2008-01-10T00:00:00",
        "Bank": "C",
        "Stock Price": 281.1000061035156
      },
      {
        "Date": "2008-01-11T00:00:00",
        "Bank": "C",
        "Stock Price": 285.6000061035156
      },
      {
        "Date": "2008-01-14T00:00:00",
        "Bank": "C",
        "Stock Price": 290.6000061035156
      },
      {
        "Date": "2008-01-15T00:00:00",
        "Bank": "C",
        "Stock Price": 269.3999938964844
      },
      {
        "Date": "2008-01-16T00:00:00",
        "Bank": "C",
        "Stock Price": 262.3999938964844
      },
      {
        "Date": "2008-01-17T00:00:00",
        "Bank": "C",
        "Stock Price": 249.60000610351562
      },
      {"Date": "2008-01-18T00:00:00", "Bank": "C", "Stock Price": 244.5},
      {"Date": "2008-01-22T00:00:00", "Bank": "C", "Stock Price": 244},
      {
        "Date": "2008-01-23T00:00:00",
        "Bank": "C",
        "Stock Price": 263.6000061035156
      },
      {
        "Date": "2008-01-24T00:00:00",
        "Bank": "C",
        "Stock Price": 273.29998779296875
      },
      {
        "Date": "2008-01-25T00:00:00",
        "Bank": "C",
        "Stock Price": 266.3999938964844
      },
      {"Date": "2008-01-28T00:00:00", "Bank": "C", "Stock Price": 276.5},
      {
        "Date": "2008-01-29T00:00:00",
        "Bank": "C",
        "Stock Price": 279.1000061035156
      },
      {
        "Date": "2008-01-30T00:00:00",
        "Bank": "C",
        "Stock Price": 278.79998779296875
      },
      {
        "Date": "2008-01-31T00:00:00",
        "Bank": "C",
        "Stock Price": 281.70001220703125
      },
      {
        "Date": "2008-02-01T00:00:00",
        "Bank": "C",
        "Stock Price": 296.8999938964844
      },
      {
        "Date": "2008-02-04T00:00:00",
        "Bank": "C",
        "Stock Price": 292.20001220703125
      },
      {"Date": "2008-02-05T00:00:00", "Bank": "C", "Stock Price": 270.5},
      {
        "Date": "2008-02-06T00:00:00",
        "Bank": "C",
        "Stock Price": 269.20001220703125
      },
      {"Date": "2008-02-07T00:00:00", "Bank": "C", "Stock Price": 267},
      {
        "Date": "2008-02-08T00:00:00",
        "Bank": "C",
        "Stock Price": 260.29998779296875
      },
      {
        "Date": "2008-02-11T00:00:00",
        "Bank": "C",
        "Stock Price": 258.1000061035156
      },
      {
        "Date": "2008-02-12T00:00:00",
        "Bank": "C",
        "Stock Price": 262.1000061035156
      },
      {
        "Date": "2008-02-13T00:00:00",
        "Bank": "C",
        "Stock Price": 263.3999938964844
      },
      {
        "Date": "2008-02-14T00:00:00",
        "Bank": "C",
        "Stock Price": 257.3999938964844
      },
      {
        "Date": "2008-02-15T00:00:00",
        "Bank": "C",
        "Stock Price": 254.8000030517578
      },
      {
        "Date": "2008-02-19T00:00:00",
        "Bank": "C",
        "Stock Price": 253.1999969482422
      },
      {
        "Date": "2008-02-20T00:00:00",
        "Bank": "C",
        "Stock Price": 254.89999389648438
      },
      {"Date": "2008-02-21T00:00:00", "Bank": "C", "Stock Price": 250.5},
      {
        "Date": "2008-02-22T00:00:00",
        "Bank": "C",
        "Stock Price": 251.1999969482422
      },
      {
        "Date": "2008-02-25T00:00:00",
        "Bank": "C",
        "Stock Price": 247.39999389648438
      },
      {"Date": "2008-02-26T00:00:00", "Bank": "C", "Stock Price": 249.5},
      {
        "Date": "2008-02-27T00:00:00",
        "Bank": "C",
        "Stock Price": 257.20001220703125
      },
      {
        "Date": "2008-02-28T00:00:00",
        "Bank": "C",
        "Stock Price": 250.10000610351562
      },
      {
        "Date": "2008-02-29T00:00:00",
        "Bank": "C",
        "Stock Price": 237.10000610351562
      },
      {
        "Date": "2008-03-03T00:00:00",
        "Bank": "C",
        "Stock Price": 230.89999389648438
      },
      {"Date": "2008-03-04T00:00:00", "Bank": "C", "Stock Price": 221},
      {"Date": "2008-03-05T00:00:00", "Bank": "C", "Stock Price": 221.5},
      {
        "Date": "2008-03-06T00:00:00",
        "Bank": "C",
        "Stock Price": 211.6999969482422
      },
      {
        "Date": "2008-03-07T00:00:00",
        "Bank": "C",
        "Stock Price": 209.10000610351562
      },
      {
        "Date": "2008-03-10T00:00:00",
        "Bank": "C",
        "Stock Price": 196.89999389648438
      },
      {
        "Date": "2008-03-11T00:00:00",
        "Bank": "C",
        "Stock Price": 214.89999389648438
      },
      {
        "Date": "2008-03-12T00:00:00",
        "Bank": "C",
        "Stock Price": 212.10000610351562
      },
      {
        "Date": "2008-03-13T00:00:00",
        "Bank": "C",
        "Stock Price": 210.6999969482422
      },
      {
        "Date": "2008-03-14T00:00:00",
        "Bank": "C",
        "Stock Price": 197.8000030517578
      },
      {
        "Date": "2008-03-17T00:00:00",
        "Bank": "C",
        "Stock Price": 186.1999969482422
      },
      {
        "Date": "2008-03-18T00:00:00",
        "Bank": "C",
        "Stock Price": 207.10000610351562
      },
      {
        "Date": "2008-03-19T00:00:00",
        "Bank": "C",
        "Stock Price": 204.10000610351562
      },
      {"Date": "2008-03-20T00:00:00", "Bank": "C", "Stock Price": 225},
      {
        "Date": "2008-03-24T00:00:00",
        "Bank": "C",
        "Stock Price": 232.6999969482422
      },
      {
        "Date": "2008-03-25T00:00:00",
        "Bank": "C",
        "Stock Price": 234.1999969482422
      },
      {"Date": "2008-03-26T00:00:00", "Bank": "C", "Stock Price": 220.5},
      {
        "Date": "2008-03-27T00:00:00",
        "Bank": "C",
        "Stock Price": 217.89999389648438
      },
      {
        "Date": "2008-03-28T00:00:00",
        "Bank": "C",
        "Stock Price": 208.3000030517578
      },
      {
        "Date": "2008-03-31T00:00:00",
        "Bank": "C",
        "Stock Price": 214.1999969482422
      },
      {
        "Date": "2008-04-01T00:00:00",
        "Bank": "C",
        "Stock Price": 238.39999389648438
      },
      {
        "Date": "2008-04-02T00:00:00",
        "Bank": "C",
        "Stock Price": 240.1999969482422
      },
      {
        "Date": "2008-04-03T00:00:00",
        "Bank": "C",
        "Stock Price": 243.60000610351562
      },
      {
        "Date": "2008-04-04T00:00:00",
        "Bank": "C",
        "Stock Price": 240.8000030517578
      },
      {"Date": "2008-04-07T00:00:00", "Bank": "C", "Stock Price": 246},
      {
        "Date": "2008-04-08T00:00:00",
        "Bank": "C",
        "Stock Price": 237.60000610351562
      },
      {
        "Date": "2008-04-09T00:00:00",
        "Bank": "C",
        "Stock Price": 235.8000030517578
      },
      {
        "Date": "2008-04-10T00:00:00",
        "Bank": "C",
        "Stock Price": 237.10000610351562
      },
      {
        "Date": "2008-04-11T00:00:00",
        "Bank": "C",
        "Stock Price": 233.60000610351562
      },
      {
        "Date": "2008-04-14T00:00:00",
        "Bank": "C",
        "Stock Price": 225.10000610351562
      },
      {"Date": "2008-04-15T00:00:00", "Bank": "C", "Stock Price": 228},
      {
        "Date": "2008-04-16T00:00:00",
        "Bank": "C",
        "Stock Price": 234.39999389648438
      },
      {
        "Date": "2008-04-17T00:00:00",
        "Bank": "C",
        "Stock Price": 240.3000030517578
      },
      {
        "Date": "2008-04-18T00:00:00",
        "Bank": "C",
        "Stock Price": 251.10000610351562
      },
      {
        "Date": "2008-04-21T00:00:00",
        "Bank": "C",
        "Stock Price": 250.3000030517578
      },
      {
        "Date": "2008-04-22T00:00:00",
        "Bank": "C",
        "Stock Price": 251.1999969482422
      },
      {
        "Date": "2008-04-23T00:00:00",
        "Bank": "C",
        "Stock Price": 246.3000030517578
      },
      {
        "Date": "2008-04-24T00:00:00",
        "Bank": "C",
        "Stock Price": 257.6000061035156
      },
      {"Date": "2008-04-25T00:00:00", "Bank": "C", "Stock Price": 266},
      {
        "Date": "2008-04-28T00:00:00",
        "Bank": "C",
        "Stock Price": 268.1000061035156
      },
      {
        "Date": "2008-04-29T00:00:00",
        "Bank": "C",
        "Stock Price": 263.20001220703125
      },
      {
        "Date": "2008-04-30T00:00:00",
        "Bank": "C",
        "Stock Price": 252.6999969482422
      },
      {
        "Date": "2008-05-01T00:00:00",
        "Bank": "C",
        "Stock Price": 259.8999938964844
      },
      {
        "Date": "2008-05-02T00:00:00",
        "Bank": "C",
        "Stock Price": 263.8999938964844
      },
      {"Date": "2008-05-05T00:00:00", "Bank": "C", "Stock Price": 257.5},
      {
        "Date": "2008-05-06T00:00:00",
        "Bank": "C",
        "Stock Price": 258.70001220703125
      },
      {
        "Date": "2008-05-07T00:00:00",
        "Bank": "C",
        "Stock Price": 244.8000030517578
      },
      {"Date": "2008-05-08T00:00:00", "Bank": "C", "Stock Price": 243},
      {
        "Date": "2008-05-09T00:00:00",
        "Bank": "C",
        "Stock Price": 236.3000030517578
      },
      {
        "Date": "2008-05-12T00:00:00",
        "Bank": "C",
        "Stock Price": 236.39999389648438
      },
      {
        "Date": "2008-05-13T00:00:00",
        "Bank": "C",
        "Stock Price": 230.3000030517578
      },
      {"Date": "2008-05-14T00:00:00", "Bank": "C", "Stock Price": 232.5},
      {
        "Date": "2008-05-15T00:00:00",
        "Bank": "C",
        "Stock Price": 237.3000030517578
      },
      {
        "Date": "2008-05-16T00:00:00",
        "Bank": "C",
        "Stock Price": 231.1999969482422
      },
      {
        "Date": "2008-05-19T00:00:00",
        "Bank": "C",
        "Stock Price": 229.89999389648438
      },
      {
        "Date": "2008-05-20T00:00:00",
        "Bank": "C",
        "Stock Price": 221.10000610351562
      },
      {
        "Date": "2008-05-21T00:00:00",
        "Bank": "C",
        "Stock Price": 210.60000610351562
      },
      {
        "Date": "2008-05-22T00:00:00",
        "Bank": "C",
        "Stock Price": 217.1999969482422
      },
      {
        "Date": "2008-05-23T00:00:00",
        "Bank": "C",
        "Stock Price": 211.1999969482422
      },
      {
        "Date": "2008-05-27T00:00:00",
        "Bank": "C",
        "Stock Price": 216.60000610351562
      },
      {"Date": "2008-05-28T00:00:00", "Bank": "C", "Stock Price": 216},
      {
        "Date": "2008-05-29T00:00:00",
        "Bank": "C",
        "Stock Price": 220.39999389648438
      },
      {
        "Date": "2008-05-30T00:00:00",
        "Bank": "C",
        "Stock Price": 218.89999389648438
      },
      {
        "Date": "2008-06-02T00:00:00",
        "Bank": "C",
        "Stock Price": 214.60000610351562
      },
      {
        "Date": "2008-06-03T00:00:00",
        "Bank": "C",
        "Stock Price": 214.1999969482422
      },
      {
        "Date": "2008-06-04T00:00:00",
        "Bank": "C",
        "Stock Price": 210.8000030517578
      },
      {
        "Date": "2008-06-05T00:00:00",
        "Bank": "C",
        "Stock Price": 212.1999969482422
      },
      {
        "Date": "2008-06-06T00:00:00",
        "Bank": "C",
        "Stock Price": 200.60000610351562
      },
      {"Date": "2008-06-09T00:00:00", "Bank": "C", "Stock Price": 196},
      {
        "Date": "2008-06-10T00:00:00",
        "Bank": "C",
        "Stock Price": 202.60000610351562
      },
      {
        "Date": "2008-06-11T00:00:00",
        "Bank": "C",
        "Stock Price": 192.10000610351562
      },
      {
        "Date": "2008-06-12T00:00:00",
        "Bank": "C",
        "Stock Price": 198.89999389648438
      },
      {
        "Date": "2008-06-13T00:00:00",
        "Bank": "C",
        "Stock Price": 204.8000030517578
      },
      {
        "Date": "2008-06-16T00:00:00",
        "Bank": "C",
        "Stock Price": 208.3000030517578
      },
      {
        "Date": "2008-06-17T00:00:00",
        "Bank": "C",
        "Stock Price": 204.60000610351562
      },
      {"Date": "2008-06-18T00:00:00", "Bank": "C", "Stock Price": 204},
      {
        "Date": "2008-06-19T00:00:00",
        "Bank": "C",
        "Stock Price": 201.6999969482422
      },
      {"Date": "2008-06-20T00:00:00", "Bank": "C", "Stock Price": 193},
      {"Date": "2008-06-23T00:00:00", "Bank": "C", "Stock Price": 185.5},
      {"Date": "2008-06-24T00:00:00", "Bank": "C", "Stock Price": 188.5},
      {"Date": "2008-06-25T00:00:00", "Bank": "C", "Stock Price": 188.5},
      {
        "Date": "2008-06-26T00:00:00",
        "Bank": "C",
        "Stock Price": 176.6999969482422
      },
      {"Date": "2008-06-27T00:00:00", "Bank": "C", "Stock Price": 172.5},
      {
        "Date": "2008-06-30T00:00:00",
        "Bank": "C",
        "Stock Price": 167.60000610351562
      },
      {
        "Date": "2008-07-01T00:00:00",
        "Bank": "C",
        "Stock Price": 171.3000030517578
      },
      {
        "Date": "2008-07-02T00:00:00",
        "Bank": "C",
        "Stock Price": 168.39999389648438
      },
      {
        "Date": "2008-07-03T00:00:00",
        "Bank": "C",
        "Stock Price": 168.1999969482422
      },
      {"Date": "2008-07-07T00:00:00", "Bank": "C", "Stock Price": 164},
      {
        "Date": "2008-07-08T00:00:00",
        "Bank": "C",
        "Stock Price": 173.89999389648438
      },
      {
        "Date": "2008-07-09T00:00:00",
        "Bank": "C",
        "Stock Price": 164.39999389648438
      },
      {
        "Date": "2008-07-10T00:00:00",
        "Bank": "C",
        "Stock Price": 162.8000030517578
      },
      {
        "Date": "2008-07-11T00:00:00",
        "Bank": "C",
        "Stock Price": 161.89999389648438
      },
      {
        "Date": "2008-07-14T00:00:00",
        "Bank": "C",
        "Stock Price": 152.1999969482422
      },
      {
        "Date": "2008-07-15T00:00:00",
        "Bank": "C",
        "Stock Price": 145.60000610351562
      },
      {
        "Date": "2008-07-16T00:00:00",
        "Bank": "C",
        "Stock Price": 164.6999969482422
      },
      {
        "Date": "2008-07-17T00:00:00",
        "Bank": "C",
        "Stock Price": 179.6999969482422
      },
      {"Date": "2008-07-18T00:00:00", "Bank": "C", "Stock Price": 193.5},
      {
        "Date": "2008-07-21T00:00:00",
        "Bank": "C",
        "Stock Price": 196.89999389648438
      },
      {
        "Date": "2008-07-22T00:00:00",
        "Bank": "C",
        "Stock Price": 208.89999389648438
      },
      {
        "Date": "2008-07-23T00:00:00",
        "Bank": "C",
        "Stock Price": 211.1999969482422
      },
      {
        "Date": "2008-07-24T00:00:00",
        "Bank": "C",
        "Stock Price": 190.60000610351562
      },
      {"Date": "2008-07-25T00:00:00", "Bank": "C", "Stock Price": 188.5},
      {
        "Date": "2008-07-28T00:00:00",
        "Bank": "C",
        "Stock Price": 174.3000030517578
      },
      {"Date": "2008-07-29T00:00:00", "Bank": "C", "Stock Price": 184.5},
      {
        "Date": "2008-07-30T00:00:00",
        "Bank": "C",
        "Stock Price": 188.10000610351562
      },
      {
        "Date": "2008-07-31T00:00:00",
        "Bank": "C",
        "Stock Price": 186.89999389648438
      },
      {
        "Date": "2008-08-01T00:00:00",
        "Bank": "C",
        "Stock Price": 188.6999969482422
      },
      {
        "Date": "2008-08-04T00:00:00",
        "Bank": "C",
        "Stock Price": 188.3000030517578
      },
      {
        "Date": "2008-08-05T00:00:00",
        "Bank": "C",
        "Stock Price": 199.1999969482422
      },
      {"Date": "2008-08-06T00:00:00", "Bank": "C", "Stock Price": 197},
      {
        "Date": "2008-08-07T00:00:00",
        "Bank": "C",
        "Stock Price": 184.6999969482422
      },
      {
        "Date": "2008-08-08T00:00:00",
        "Bank": "C",
        "Stock Price": 193.89999389648438
      },
      {
        "Date": "2008-08-11T00:00:00",
        "Bank": "C",
        "Stock Price": 198.1999969482422
      },
      {
        "Date": "2008-08-12T00:00:00",
        "Bank": "C",
        "Stock Price": 185.39999389648438
      },
      {
        "Date": "2008-08-13T00:00:00",
        "Bank": "C",
        "Stock Price": 178.10000610351562
      },
      {
        "Date": "2008-08-14T00:00:00",
        "Bank": "C",
        "Stock Price": 180.8000030517578
      },
      {"Date": "2008-08-15T00:00:00", "Bank": "C", "Stock Price": 185.5},
      {
        "Date": "2008-08-18T00:00:00",
        "Bank": "C",
        "Stock Price": 176.1999969482422
      },
      {
        "Date": "2008-08-19T00:00:00",
        "Bank": "C",
        "Stock Price": 171.89999389648438
      },
      {
        "Date": "2008-08-20T00:00:00",
        "Bank": "C",
        "Stock Price": 174.89999389648438
      },
      {
        "Date": "2008-08-21T00:00:00",
        "Bank": "C",
        "Stock Price": 174.6999969482422
      },
      {
        "Date": "2008-08-22T00:00:00",
        "Bank": "C",
        "Stock Price": 181.39999389648438
      },
      {
        "Date": "2008-08-25T00:00:00",
        "Bank": "C",
        "Stock Price": 176.10000610351562
      },
      {
        "Date": "2008-08-26T00:00:00",
        "Bank": "C",
        "Stock Price": 178.39999389648438
      },
      {
        "Date": "2008-08-27T00:00:00",
        "Bank": "C",
        "Stock Price": 181.1999969482422
      },
      {
        "Date": "2008-08-28T00:00:00",
        "Bank": "C",
        "Stock Price": 190.8000030517578
      },
      {
        "Date": "2008-08-29T00:00:00",
        "Bank": "C",
        "Stock Price": 189.89999389648438
      },
      {
        "Date": "2008-09-02T00:00:00",
        "Bank": "C",
        "Stock Price": 191.10000610351562
      },
      {
        "Date": "2008-09-03T00:00:00",
        "Bank": "C",
        "Stock Price": 196.10000610351562
      },
      {"Date": "2008-09-04T00:00:00", "Bank": "C", "Stock Price": 183},
      {
        "Date": "2008-09-05T00:00:00",
        "Bank": "C",
        "Stock Price": 190.6999969482422
      },
      {
        "Date": "2008-09-08T00:00:00",
        "Bank": "C",
        "Stock Price": 203.1999969482422
      },
      {
        "Date": "2008-09-09T00:00:00",
        "Bank": "C",
        "Stock Price": 188.8000030517578
      },
      {
        "Date": "2008-09-10T00:00:00",
        "Bank": "C",
        "Stock Price": 186.8000030517578
      },
      {
        "Date": "2008-09-11T00:00:00",
        "Bank": "C",
        "Stock Price": 186.10000610351562
      },
      {
        "Date": "2008-09-12T00:00:00",
        "Bank": "C",
        "Stock Price": 179.60000610351562
      },
      {
        "Date": "2008-09-15T00:00:00",
        "Bank": "C",
        "Stock Price": 152.39999389648438
      },
      {"Date": "2008-09-16T00:00:00", "Bank": "C", "Stock Price": 157.5},
      {
        "Date": "2008-09-17T00:00:00",
        "Bank": "C",
        "Stock Price": 140.3000030517578
      },
      {"Date": "2008-09-18T00:00:00", "Bank": "C", "Stock Price": 166.5},
      {"Date": "2008-09-19T00:00:00", "Bank": "C", "Stock Price": 206.5},
      {
        "Date": "2008-09-22T00:00:00",
        "Bank": "C",
        "Stock Price": 200.10000610351562
      },
      {
        "Date": "2008-09-23T00:00:00",
        "Bank": "C",
        "Stock Price": 199.89999389648438
      },
      {
        "Date": "2008-09-24T00:00:00",
        "Bank": "C",
        "Stock Price": 189.60000610351562
      },
      {
        "Date": "2008-09-25T00:00:00",
        "Bank": "C",
        "Stock Price": 194.10000610351562
      },
      {"Date": "2008-09-26T00:00:00", "Bank": "C", "Stock Price": 201.5},
      {"Date": "2008-09-29T00:00:00", "Bank": "C", "Stock Price": 177.5},
      {
        "Date": "2008-09-30T00:00:00",
        "Bank": "C",
        "Stock Price": 205.10000610351562
      },
      {"Date": "2008-10-01T00:00:00", "Bank": "C", "Stock Price": 230},
      {"Date": "2008-10-02T00:00:00", "Bank": "C", "Stock Price": 225},
      {"Date": "2008-10-03T00:00:00", "Bank": "C", "Stock Price": 183.5},
      {
        "Date": "2008-10-06T00:00:00",
        "Bank": "C",
        "Stock Price": 174.10000610351562
      },
      {"Date": "2008-10-07T00:00:00", "Bank": "C", "Stock Price": 151.5},
      {"Date": "2008-10-08T00:00:00", "Bank": "C", "Stock Price": 144},
      {
        "Date": "2008-10-09T00:00:00",
        "Bank": "C",
        "Stock Price": 129.3000030517578
      },
      {
        "Date": "2008-10-10T00:00:00",
        "Bank": "C",
        "Stock Price": 141.10000610351562
      },
      {"Date": "2008-10-13T00:00:00", "Bank": "C", "Stock Price": 157.5},
      {
        "Date": "2008-10-14T00:00:00",
        "Bank": "C",
        "Stock Price": 186.1999969482422
      },
      {
        "Date": "2008-10-15T00:00:00",
        "Bank": "C",
        "Stock Price": 162.3000030517578
      },
      {"Date": "2008-10-16T00:00:00", "Bank": "C", "Stock Price": 159},
      {
        "Date": "2008-10-17T00:00:00",
        "Bank": "C",
        "Stock Price": 148.8000030517578
      },
      {
        "Date": "2008-10-20T00:00:00",
        "Bank": "C",
        "Stock Price": 150.89999389648438
      },
      {
        "Date": "2008-10-21T00:00:00",
        "Bank": "C",
        "Stock Price": 141.8000030517578
      },
      {
        "Date": "2008-10-22T00:00:00",
        "Bank": "C",
        "Stock Price": 133.1999969482422
      },
      {
        "Date": "2008-10-23T00:00:00",
        "Bank": "C",
        "Stock Price": 131.10000610351562
      },
      {
        "Date": "2008-10-24T00:00:00",
        "Bank": "C",
        "Stock Price": 121.4000015258789
      },
      {
        "Date": "2008-10-27T00:00:00",
        "Bank": "C",
        "Stock Price": 117.30000305175781
      },
      {
        "Date": "2008-10-28T00:00:00",
        "Bank": "C",
        "Stock Price": 134.10000610351562
      },
      {
        "Date": "2008-10-29T00:00:00",
        "Bank": "C",
        "Stock Price": 129.10000610351562
      },
      {
        "Date": "2008-10-30T00:00:00",
        "Bank": "C",
        "Stock Price": 131.10000610351562
      },
      {"Date": "2008-10-31T00:00:00", "Bank": "C", "Stock Price": 136.5},
      {
        "Date": "2008-11-03T00:00:00",
        "Bank": "C",
        "Stock Price": 139.89999389648438
      },
      {
        "Date": "2008-11-04T00:00:00",
        "Bank": "C",
        "Stock Price": 146.8000030517578
      },
      {
        "Date": "2008-11-05T00:00:00",
        "Bank": "C",
        "Stock Price": 126.30000305175781
      },
      {
        "Date": "2008-11-06T00:00:00",
        "Bank": "C",
        "Stock Price": 115.19999694824219
      },
      {
        "Date": "2008-11-07T00:00:00",
        "Bank": "C",
        "Stock Price": 118.19999694824219
      },
      {
        "Date": "2008-11-10T00:00:00",
        "Bank": "C",
        "Stock Price": 112.0999984741211
      },
      {"Date": "2008-11-11T00:00:00", "Bank": "C", "Stock Price": 108},
      {
        "Date": "2008-11-12T00:00:00",
        "Bank": "C",
        "Stock Price": 96.4000015258789
      },
      {"Date": "2008-11-13T00:00:00", "Bank": "C", "Stock Price": 94.5},
      {
        "Date": "2008-11-14T00:00:00",
        "Bank": "C",
        "Stock Price": 95.19999694824219
      },
      {
        "Date": "2008-11-17T00:00:00",
        "Bank": "C",
        "Stock Price": 88.9000015258789
      },
      {
        "Date": "2008-11-18T00:00:00",
        "Bank": "C",
        "Stock Price": 83.5999984741211
      },
      {"Date": "2008-11-19T00:00:00", "Bank": "C", "Stock Price": 64},
      {
        "Date": "2008-11-20T00:00:00",
        "Bank": "C",
        "Stock Price": 47.099998474121094
      },
      {
        "Date": "2008-11-21T00:00:00",
        "Bank": "C",
        "Stock Price": 37.70000076293945
      },
      {"Date": "2008-11-24T00:00:00", "Bank": "C", "Stock Price": 59.5},
      {
        "Date": "2008-11-25T00:00:00",
        "Bank": "C",
        "Stock Price": 60.79999923706055
      },
      {"Date": "2008-11-26T00:00:00", "Bank": "C", "Stock Price": 70.5},
      {
        "Date": "2008-11-28T00:00:00",
        "Bank": "C",
        "Stock Price": 82.9000015258789
      },
      {"Date": "2008-12-01T00:00:00", "Bank": "C", "Stock Price": 64.5},
      {
        "Date": "2008-12-02T00:00:00",
        "Bank": "C",
        "Stock Price": 72.19999694824219
      },
      {
        "Date": "2008-12-03T00:00:00",
        "Bank": "C",
        "Stock Price": 78.19999694824219
      },
      {"Date": "2008-12-04T00:00:00", "Bank": "C", "Stock Price": 74},
      {
        "Date": "2008-12-05T00:00:00",
        "Bank": "C",
        "Stock Price": 77.0999984741211
      },
      {
        "Date": "2008-12-08T00:00:00",
        "Bank": "C",
        "Stock Price": 84.69999694824219
      },
      {
        "Date": "2008-12-09T00:00:00",
        "Bank": "C",
        "Stock Price": 85.4000015258789
      },
      {"Date": "2008-12-10T00:00:00", "Bank": "C", "Stock Price": 83},
      {
        "Date": "2008-12-11T00:00:00",
        "Bank": "C",
        "Stock Price": 75.69999694824219
      },
      {"Date": "2008-12-12T00:00:00", "Bank": "C", "Stock Price": 77},
      {"Date": "2008-12-15T00:00:00", "Bank": "C", "Stock Price": 74},
      {
        "Date": "2008-12-16T00:00:00",
        "Bank": "C",
        "Stock Price": 82.30000305175781
      },
      {
        "Date": "2008-12-17T00:00:00",
        "Bank": "C",
        "Stock Price": 78.30000305175781
      },
      {
        "Date": "2008-12-18T00:00:00",
        "Bank": "C",
        "Stock Price": 74.30000305175781
      },
      {
        "Date": "2008-12-19T00:00:00",
        "Bank": "C",
        "Stock Price": 70.19999694824219
      },
      {"Date": "2008-12-22T00:00:00", "Bank": "C", "Stock Price": 67.5},
      {
        "Date": "2008-12-23T00:00:00",
        "Bank": "C",
        "Stock Price": 65.19999694824219
      },
      {
        "Date": "2008-12-24T00:00:00",
        "Bank": "C",
        "Stock Price": 67.80000305175781
      },
      {
        "Date": "2008-12-26T00:00:00",
        "Bank": "C",
        "Stock Price": 67.30000305175781
      },
      {
        "Date": "2008-12-29T00:00:00",
        "Bank": "C",
        "Stock Price": 65.69999694824219
      },
      {"Date": "2008-12-30T00:00:00", "Bank": "C", "Stock Price": 68},
      {
        "Date": "2008-12-31T00:00:00",
        "Bank": "C",
        "Stock Price": 67.0999984741211
      },
      {
        "Date": "2009-01-02T00:00:00",
        "Bank": "C",
        "Stock Price": 71.4000015258789
      },
      {
        "Date": "2009-01-05T00:00:00",
        "Bank": "C",
        "Stock Price": 70.80000305175781
      },
      {
        "Date": "2009-01-06T00:00:00",
        "Bank": "C",
        "Stock Price": 74.5999984741211
      },
      {"Date": "2009-01-07T00:00:00", "Bank": "C", "Stock Price": 71.5},
      {
        "Date": "2009-01-08T00:00:00",
        "Bank": "C",
        "Stock Price": 71.5999984741211
      },
      {"Date": "2009-01-09T00:00:00", "Bank": "C", "Stock Price": 67.5},
      {"Date": "2009-01-12T00:00:00", "Bank": "C", "Stock Price": 56},
      {"Date": "2009-01-13T00:00:00", "Bank": "C", "Stock Price": 59},
      {
        "Date": "2009-01-14T00:00:00",
        "Bank": "C",
        "Stock Price": 45.29999923706055
      },
      {
        "Date": "2009-01-15T00:00:00",
        "Bank": "C",
        "Stock Price": 38.29999923706055
      },
      {"Date": "2009-01-16T00:00:00", "Bank": "C", "Stock Price": 35},
      {"Date": "2009-01-20T00:00:00", "Bank": "C", "Stock Price": 28},
      {
        "Date": "2009-01-21T00:00:00",
        "Bank": "C",
        "Stock Price": 36.70000076293945
      },
      {
        "Date": "2009-01-22T00:00:00",
        "Bank": "C",
        "Stock Price": 31.100000381469727
      },
      {
        "Date": "2009-01-23T00:00:00",
        "Bank": "C",
        "Stock Price": 34.70000076293945
      },
      {
        "Date": "2009-01-26T00:00:00",
        "Bank": "C",
        "Stock Price": 33.29999923706055
      },
      {"Date": "2009-01-27T00:00:00", "Bank": "C", "Stock Price": 35.5},
      {
        "Date": "2009-01-28T00:00:00",
        "Bank": "C",
        "Stock Price": 42.099998474121094
      },
      {"Date": "2009-01-29T00:00:00", "Bank": "C", "Stock Price": 39},
      {"Date": "2009-01-30T00:00:00", "Bank": "C", "Stock Price": 35.5},
      {"Date": "2009-02-02T00:00:00", "Bank": "C", "Stock Price": 36.5},
      {
        "Date": "2009-02-03T00:00:00",
        "Bank": "C",
        "Stock Price": 34.599998474121094
      },
      {
        "Date": "2009-02-04T00:00:00",
        "Bank": "C",
        "Stock Price": 34.900001525878906
      },
      {
        "Date": "2009-02-05T00:00:00",
        "Bank": "C",
        "Stock Price": 35.29999923706055
      },
      {
        "Date": "2009-02-06T00:00:00",
        "Bank": "C",
        "Stock Price": 39.099998474121094
      },
      {"Date": "2009-02-09T00:00:00", "Bank": "C", "Stock Price": 39.5},
      {"Date": "2009-02-10T00:00:00", "Bank": "C", "Stock Price": 33.5},
      {
        "Date": "2009-02-11T00:00:00",
        "Bank": "C",
        "Stock Price": 36.900001525878906
      },
      {
        "Date": "2009-02-12T00:00:00",
        "Bank": "C",
        "Stock Price": 36.099998474121094
      },
      {
        "Date": "2009-02-13T00:00:00",
        "Bank": "C",
        "Stock Price": 34.900001525878906
      },
      {
        "Date": "2009-02-17T00:00:00",
        "Bank": "C",
        "Stock Price": 30.600000381469727
      },
      {
        "Date": "2009-02-18T00:00:00",
        "Bank": "C",
        "Stock Price": 29.100000381469727
      },
      {
        "Date": "2009-02-19T00:00:00",
        "Bank": "C",
        "Stock Price": 25.100000381469727
      },
      {"Date": "2009-02-20T00:00:00", "Bank": "C", "Stock Price": 19.5},
      {
        "Date": "2009-02-23T00:00:00",
        "Bank": "C",
        "Stock Price": 21.399999618530273
      },
      {"Date": "2009-02-24T00:00:00", "Bank": "C", "Stock Price": 26},
      {
        "Date": "2009-02-25T00:00:00",
        "Bank": "C",
        "Stock Price": 25.200000762939453
      },
      {
        "Date": "2009-02-26T00:00:00",
        "Bank": "C",
        "Stock Price": 24.600000381469727
      },
      {"Date": "2009-02-27T00:00:00", "Bank": "C", "Stock Price": 15},
      {"Date": "2009-03-02T00:00:00", "Bank": "C", "Stock Price": 12},
      {
        "Date": "2009-03-03T00:00:00",
        "Bank": "C",
        "Stock Price": 12.199999809265137
      },
      {
        "Date": "2009-03-04T00:00:00",
        "Bank": "C",
        "Stock Price": 11.300000190734863
      },
      {
        "Date": "2009-03-05T00:00:00",
        "Bank": "C",
        "Stock Price": 10.199999809265137
      },
      {
        "Date": "2009-03-06T00:00:00",
        "Bank": "C",
        "Stock Price": 10.300000190734863
      },
      {"Date": "2009-03-09T00:00:00", "Bank": "C", "Stock Price": 10.5},
      {"Date": "2009-03-10T00:00:00", "Bank": "C", "Stock Price": 14.5},
      {
        "Date": "2009-03-11T00:00:00",
        "Bank": "C",
        "Stock Price": 15.399999618530273
      },
      {
        "Date": "2009-03-12T00:00:00",
        "Bank": "C",
        "Stock Price": 16.700000762939453
      },
      {
        "Date": "2009-03-13T00:00:00",
        "Bank": "C",
        "Stock Price": 17.799999237060547
      },
      {
        "Date": "2009-03-16T00:00:00",
        "Bank": "C",
        "Stock Price": 23.299999237060547
      },
      {
        "Date": "2009-03-17T00:00:00",
        "Bank": "C",
        "Stock Price": 25.100000381469727
      },
      {
        "Date": "2009-03-18T00:00:00",
        "Bank": "C",
        "Stock Price": 30.799999237060547
      },
      {"Date": "2009-03-19T00:00:00", "Bank": "C", "Stock Price": 26},
      {
        "Date": "2009-03-20T00:00:00",
        "Bank": "C",
        "Stock Price": 26.200000762939453
      },
      {
        "Date": "2009-03-23T00:00:00",
        "Bank": "C",
        "Stock Price": 31.299999237060547
      },
      {
        "Date": "2009-03-24T00:00:00",
        "Bank": "C",
        "Stock Price": 30.100000381469727
      },
      {"Date": "2009-03-25T00:00:00", "Bank": "C", "Stock Price": 29.5},
      {
        "Date": "2009-03-26T00:00:00",
        "Bank": "C",
        "Stock Price": 28.100000381469727
      },
      {
        "Date": "2009-03-27T00:00:00",
        "Bank": "C",
        "Stock Price": 26.200000762939453
      },
      {
        "Date": "2009-03-30T00:00:00",
        "Bank": "C",
        "Stock Price": 23.100000381469727
      },
      {
        "Date": "2009-03-31T00:00:00",
        "Bank": "C",
        "Stock Price": 25.299999237060547
      },
      {
        "Date": "2009-04-01T00:00:00",
        "Bank": "C",
        "Stock Price": 26.799999237060547
      },
      {
        "Date": "2009-04-02T00:00:00",
        "Bank": "C",
        "Stock Price": 27.399999618530273
      },
      {"Date": "2009-04-03T00:00:00", "Bank": "C", "Stock Price": 28.5},
      {
        "Date": "2009-04-06T00:00:00",
        "Bank": "C",
        "Stock Price": 27.200000762939453
      },
      {
        "Date": "2009-04-07T00:00:00",
        "Bank": "C",
        "Stock Price": 27.600000381469727
      },
      {"Date": "2009-04-08T00:00:00", "Bank": "C", "Stock Price": 27},
      {
        "Date": "2009-04-09T00:00:00",
        "Bank": "C",
        "Stock Price": 30.399999618530273
      },
      {"Date": "2009-04-13T00:00:00", "Bank": "C", "Stock Price": 38},
      {
        "Date": "2009-04-14T00:00:00",
        "Bank": "C",
        "Stock Price": 40.099998474121094
      },
      {
        "Date": "2009-04-15T00:00:00",
        "Bank": "C",
        "Stock Price": 39.70000076293945
      },
      {
        "Date": "2009-04-16T00:00:00",
        "Bank": "C",
        "Stock Price": 40.099998474121094
      },
      {"Date": "2009-04-17T00:00:00", "Bank": "C", "Stock Price": 36.5},
      {
        "Date": "2009-04-20T00:00:00",
        "Bank": "C",
        "Stock Price": 29.399999618530273
      },
      {
        "Date": "2009-04-21T00:00:00",
        "Bank": "C",
        "Stock Price": 32.400001525878906
      },
      {"Date": "2009-04-22T00:00:00", "Bank": "C", "Stock Price": 32.5},
      {"Date": "2009-04-23T00:00:00", "Bank": "C", "Stock Price": 32},
      {
        "Date": "2009-04-24T00:00:00",
        "Bank": "C",
        "Stock Price": 31.899999618530273
      },
      {
        "Date": "2009-04-27T00:00:00",
        "Bank": "C",
        "Stock Price": 30.700000762939453
      },
      {
        "Date": "2009-04-28T00:00:00",
        "Bank": "C",
        "Stock Price": 28.899999618530273
      },
      {
        "Date": "2009-04-29T00:00:00",
        "Bank": "C",
        "Stock Price": 31.200000762939453
      },
      {"Date": "2009-04-30T00:00:00", "Bank": "C", "Stock Price": 30.5},
      {
        "Date": "2009-05-01T00:00:00",
        "Bank": "C",
        "Stock Price": 29.700000762939453
      },
      {"Date": "2009-05-04T00:00:00", "Bank": "C", "Stock Price": 32},
      {
        "Date": "2009-05-05T00:00:00",
        "Bank": "C",
        "Stock Price": 33.099998474121094
      },
      {
        "Date": "2009-05-06T00:00:00",
        "Bank": "C",
        "Stock Price": 38.599998474121094
      },
      {
        "Date": "2009-05-07T00:00:00",
        "Bank": "C",
        "Stock Price": 38.099998474121094
      },
      {
        "Date": "2009-05-08T00:00:00",
        "Bank": "C",
        "Stock Price": 40.20000076293945
      },
      {
        "Date": "2009-05-11T00:00:00",
        "Bank": "C",
        "Stock Price": 38.599998474121094
      },
      {
        "Date": "2009-05-12T00:00:00",
        "Bank": "C",
        "Stock Price": 36.599998474121094
      },
      {
        "Date": "2009-05-13T00:00:00",
        "Bank": "C",
        "Stock Price": 34.099998474121094
      },
      {"Date": "2009-05-14T00:00:00", "Bank": "C", "Stock Price": 35.5},
      {
        "Date": "2009-05-15T00:00:00",
        "Bank": "C",
        "Stock Price": 34.79999923706055
      },
      {
        "Date": "2009-05-18T00:00:00",
        "Bank": "C",
        "Stock Price": 36.400001525878906
      },
      {
        "Date": "2009-05-19T00:00:00",
        "Bank": "C",
        "Stock Price": 37.70000076293945
      },
      {
        "Date": "2009-05-20T00:00:00",
        "Bank": "C",
        "Stock Price": 36.900001525878906
      },
      {
        "Date": "2009-05-21T00:00:00",
        "Bank": "C",
        "Stock Price": 37.20000076293945
      },
      {
        "Date": "2009-05-22T00:00:00",
        "Bank": "C",
        "Stock Price": 36.70000076293945
      },
      {
        "Date": "2009-05-26T00:00:00",
        "Bank": "C",
        "Stock Price": 37.70000076293945
      },
      {"Date": "2009-05-27T00:00:00", "Bank": "C", "Stock Price": 37},
      {
        "Date": "2009-05-28T00:00:00",
        "Bank": "C",
        "Stock Price": 36.70000076293945
      },
      {
        "Date": "2009-05-29T00:00:00",
        "Bank": "C",
        "Stock Price": 37.20000076293945
      },
      {
        "Date": "2009-06-01T00:00:00",
        "Bank": "C",
        "Stock Price": 36.900001525878906
      },
      {
        "Date": "2009-06-02T00:00:00",
        "Bank": "C",
        "Stock Price": 35.099998474121094
      },
      {
        "Date": "2009-06-03T00:00:00",
        "Bank": "C",
        "Stock Price": 33.900001525878906
      },
      {
        "Date": "2009-06-04T00:00:00",
        "Bank": "C",
        "Stock Price": 35.70000076293945
      },
      {
        "Date": "2009-06-05T00:00:00",
        "Bank": "C",
        "Stock Price": 34.599998474121094
      },
      {
        "Date": "2009-06-08T00:00:00",
        "Bank": "C",
        "Stock Price": 34.20000076293945
      },
      {
        "Date": "2009-06-09T00:00:00",
        "Bank": "C",
        "Stock Price": 34.099998474121094
      },
      {
        "Date": "2009-06-10T00:00:00",
        "Bank": "C",
        "Stock Price": 34.79999923706055
      },
      {
        "Date": "2009-06-11T00:00:00",
        "Bank": "C",
        "Stock Price": 34.79999923706055
      },
      {
        "Date": "2009-06-12T00:00:00",
        "Bank": "C",
        "Stock Price": 34.70000076293945
      },
      {
        "Date": "2009-06-15T00:00:00",
        "Bank": "C",
        "Stock Price": 33.70000076293945
      },
      {"Date": "2009-06-16T00:00:00", "Bank": "C", "Stock Price": 32.5},
      {
        "Date": "2009-06-17T00:00:00",
        "Bank": "C",
        "Stock Price": 30.799999237060547
      },
      {
        "Date": "2009-06-18T00:00:00",
        "Bank": "C",
        "Stock Price": 31.299999237060547
      },
      {
        "Date": "2009-06-19T00:00:00",
        "Bank": "C",
        "Stock Price": 31.700000762939453
      },
      {"Date": "2009-06-22T00:00:00", "Bank": "C", "Stock Price": 30},
      {
        "Date": "2009-06-23T00:00:00",
        "Bank": "C",
        "Stock Price": 30.100000381469727
      },
      {
        "Date": "2009-06-24T00:00:00",
        "Bank": "C",
        "Stock Price": 30.399999618530273
      },
      {
        "Date": "2009-06-25T00:00:00",
        "Bank": "C",
        "Stock Price": 30.299999237060547
      },
      {
        "Date": "2009-06-26T00:00:00",
        "Bank": "C",
        "Stock Price": 30.299999237060547
      },
      {
        "Date": "2009-06-29T00:00:00",
        "Bank": "C",
        "Stock Price": 30.200000762939453
      },
      {
        "Date": "2009-06-30T00:00:00",
        "Bank": "C",
        "Stock Price": 29.700000762939453
      },
      {
        "Date": "2009-07-01T00:00:00",
        "Bank": "C",
        "Stock Price": 29.700000762939453
      },
      {
        "Date": "2009-07-02T00:00:00",
        "Bank": "C",
        "Stock Price": 28.799999237060547
      },
      {
        "Date": "2009-07-06T00:00:00",
        "Bank": "C",
        "Stock Price": 27.899999618530273
      },
      {
        "Date": "2009-07-07T00:00:00",
        "Bank": "C",
        "Stock Price": 26.899999618530273
      },
      {
        "Date": "2009-07-08T00:00:00",
        "Bank": "C",
        "Stock Price": 26.200000762939453
      },
      {
        "Date": "2009-07-09T00:00:00",
        "Bank": "C",
        "Stock Price": 26.899999618530273
      },
      {
        "Date": "2009-07-10T00:00:00",
        "Bank": "C",
        "Stock Price": 25.899999618530273
      },
      {
        "Date": "2009-07-13T00:00:00",
        "Bank": "C",
        "Stock Price": 27.799999237060547
      },
      {
        "Date": "2009-07-14T00:00:00",
        "Bank": "C",
        "Stock Price": 29.200000762939453
      },
      {
        "Date": "2009-07-15T00:00:00",
        "Bank": "C",
        "Stock Price": 31.700000762939453
      },
      {
        "Date": "2009-07-16T00:00:00",
        "Bank": "C",
        "Stock Price": 30.299999237060547
      },
      {
        "Date": "2009-07-17T00:00:00",
        "Bank": "C",
        "Stock Price": 30.200000762939453
      },
      {
        "Date": "2009-07-20T00:00:00",
        "Bank": "C",
        "Stock Price": 27.899999618530273
      },
      {"Date": "2009-07-21T00:00:00", "Bank": "C", "Stock Price": 26.5},
      {"Date": "2009-07-22T00:00:00", "Bank": "C", "Stock Price": 28},
      {
        "Date": "2009-07-23T00:00:00",
        "Bank": "C",
        "Stock Price": 27.700000762939453
      },
      {
        "Date": "2009-07-24T00:00:00",
        "Bank": "C",
        "Stock Price": 27.299999237060547
      },
      {
        "Date": "2009-07-27T00:00:00",
        "Bank": "C",
        "Stock Price": 26.899999618530273
      },
      {
        "Date": "2009-07-28T00:00:00",
        "Bank": "C",
        "Stock Price": 29.700000762939453
      },
      {
        "Date": "2009-07-29T00:00:00",
        "Bank": "C",
        "Stock Price": 32.20000076293945
      },
      {
        "Date": "2009-07-30T00:00:00",
        "Bank": "C",
        "Stock Price": 31.399999618530273
      },
      {
        "Date": "2009-07-31T00:00:00",
        "Bank": "C",
        "Stock Price": 31.700000762939453
      },
      {
        "Date": "2009-08-03T00:00:00",
        "Bank": "C",
        "Stock Price": 31.799999237060547
      },
      {"Date": "2009-08-04T00:00:00", "Bank": "C", "Stock Price": 32.5},
      {
        "Date": "2009-08-05T00:00:00",
        "Bank": "C",
        "Stock Price": 35.79999923706055
      },
      {"Date": "2009-08-06T00:00:00", "Bank": "C", "Stock Price": 38},
      {"Date": "2009-08-07T00:00:00", "Bank": "C", "Stock Price": 38.5},
      {
        "Date": "2009-08-10T00:00:00",
        "Bank": "C",
        "Stock Price": 39.400001525878906
      },
      {
        "Date": "2009-08-11T00:00:00",
        "Bank": "C",
        "Stock Price": 36.900001525878906
      },
      {
        "Date": "2009-08-12T00:00:00",
        "Bank": "C",
        "Stock Price": 39.79999923706055
      },
      {
        "Date": "2009-08-13T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2009-08-14T00:00:00",
        "Bank": "C",
        "Stock Price": 40.400001525878906
      },
      {"Date": "2009-08-17T00:00:00", "Bank": "C", "Stock Price": 40},
      {
        "Date": "2009-08-18T00:00:00",
        "Bank": "C",
        "Stock Price": 41.400001525878906
      },
      {
        "Date": "2009-08-19T00:00:00",
        "Bank": "C",
        "Stock Price": 41.29999923706055
      },
      {
        "Date": "2009-08-20T00:00:00",
        "Bank": "C",
        "Stock Price": 44.79999923706055
      },
      {"Date": "2009-08-21T00:00:00", "Bank": "C", "Stock Price": 47},
      {
        "Date": "2009-08-24T00:00:00",
        "Bank": "C",
        "Stock Price": 48.20000076293945
      },
      {"Date": "2009-08-25T00:00:00", "Bank": "C", "Stock Price": 47.5},
      {
        "Date": "2009-08-26T00:00:00",
        "Bank": "C",
        "Stock Price": 46.29999923706055
      },
      {"Date": "2009-08-27T00:00:00", "Bank": "C", "Stock Price": 50.5},
      {
        "Date": "2009-08-28T00:00:00",
        "Bank": "C",
        "Stock Price": 52.29999923706055
      },
      {"Date": "2009-08-31T00:00:00", "Bank": "C", "Stock Price": 50},
      {
        "Date": "2009-09-01T00:00:00",
        "Bank": "C",
        "Stock Price": 45.400001525878906
      },
      {
        "Date": "2009-09-02T00:00:00",
        "Bank": "C",
        "Stock Price": 45.599998474121094
      },
      {
        "Date": "2009-09-03T00:00:00",
        "Bank": "C",
        "Stock Price": 47.70000076293945
      },
      {"Date": "2009-09-04T00:00:00", "Bank": "C", "Stock Price": 48.5},
      {
        "Date": "2009-09-08T00:00:00",
        "Bank": "C",
        "Stock Price": 46.79999923706055
      },
      {
        "Date": "2009-09-09T00:00:00",
        "Bank": "C",
        "Stock Price": 46.599998474121094
      },
      {"Date": "2009-09-10T00:00:00", "Bank": "C", "Stock Price": 47.5},
      {
        "Date": "2009-09-11T00:00:00",
        "Bank": "C",
        "Stock Price": 46.099998474121094
      },
      {
        "Date": "2009-09-14T00:00:00",
        "Bank": "C",
        "Stock Price": 45.20000076293945
      },
      {
        "Date": "2009-09-15T00:00:00",
        "Bank": "C",
        "Stock Price": 41.20000076293945
      },
      {"Date": "2009-09-16T00:00:00", "Bank": "C", "Stock Price": 42},
      {
        "Date": "2009-09-17T00:00:00",
        "Bank": "C",
        "Stock Price": 44.20000076293945
      },
      {
        "Date": "2009-09-18T00:00:00",
        "Bank": "C",
        "Stock Price": 42.599998474121094
      },
      {
        "Date": "2009-09-21T00:00:00",
        "Bank": "C",
        "Stock Price": 44.29999923706055
      },
      {"Date": "2009-09-22T00:00:00", "Bank": "C", "Stock Price": 46.5},
      {
        "Date": "2009-09-23T00:00:00",
        "Bank": "C",
        "Stock Price": 45.20000076293945
      },
      {
        "Date": "2009-09-24T00:00:00",
        "Bank": "C",
        "Stock Price": 44.29999923706055
      },
      {
        "Date": "2009-09-25T00:00:00",
        "Bank": "C",
        "Stock Price": 43.79999923706055
      },
      {
        "Date": "2009-09-28T00:00:00",
        "Bank": "C",
        "Stock Price": 45.70000076293945
      },
      {"Date": "2009-09-29T00:00:00", "Bank": "C", "Stock Price": 47},
      {
        "Date": "2009-09-30T00:00:00",
        "Bank": "C",
        "Stock Price": 48.400001525878906
      },
      {
        "Date": "2009-10-01T00:00:00",
        "Bank": "C",
        "Stock Price": 45.29999923706055
      },
      {
        "Date": "2009-10-02T00:00:00",
        "Bank": "C",
        "Stock Price": 45.20000076293945
      },
      {
        "Date": "2009-10-05T00:00:00",
        "Bank": "C",
        "Stock Price": 46.70000076293945
      },
      {
        "Date": "2009-10-06T00:00:00",
        "Bank": "C",
        "Stock Price": 46.70000076293945
      },
      {
        "Date": "2009-10-07T00:00:00",
        "Bank": "C",
        "Stock Price": 46.400001525878906
      },
      {"Date": "2009-10-08T00:00:00", "Bank": "C", "Stock Price": 46.5},
      {
        "Date": "2009-10-09T00:00:00",
        "Bank": "C",
        "Stock Price": 46.29999923706055
      },
      {
        "Date": "2009-10-12T00:00:00",
        "Bank": "C",
        "Stock Price": 47.70000076293945
      },
      {
        "Date": "2009-10-13T00:00:00",
        "Bank": "C",
        "Stock Price": 48.29999923706055
      },
      {"Date": "2009-10-14T00:00:00", "Bank": "C", "Stock Price": 50},
      {"Date": "2009-10-15T00:00:00", "Bank": "C", "Stock Price": 47.5},
      {
        "Date": "2009-10-16T00:00:00",
        "Bank": "C",
        "Stock Price": 45.900001525878906
      },
      {
        "Date": "2009-10-19T00:00:00",
        "Bank": "C",
        "Stock Price": 45.400001525878906
      },
      {
        "Date": "2009-10-20T00:00:00",
        "Bank": "C",
        "Stock Price": 44.29999923706055
      },
      {
        "Date": "2009-10-21T00:00:00",
        "Bank": "C",
        "Stock Price": 44.20000076293945
      },
      {
        "Date": "2009-10-22T00:00:00",
        "Bank": "C",
        "Stock Price": 44.599998474121094
      },
      {
        "Date": "2009-10-23T00:00:00",
        "Bank": "C",
        "Stock Price": 44.599998474121094
      },
      {
        "Date": "2009-10-26T00:00:00",
        "Bank": "C",
        "Stock Price": 42.70000076293945
      },
      {
        "Date": "2009-10-27T00:00:00",
        "Bank": "C",
        "Stock Price": 42.70000076293945
      },
      {
        "Date": "2009-10-28T00:00:00",
        "Bank": "C",
        "Stock Price": 40.79999923706055
      },
      {
        "Date": "2009-10-29T00:00:00",
        "Bank": "C",
        "Stock Price": 43.099998474121094
      },
      {
        "Date": "2009-10-30T00:00:00",
        "Bank": "C",
        "Stock Price": 40.900001525878906
      },
      {
        "Date": "2009-11-02T00:00:00",
        "Bank": "C",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2009-11-03T00:00:00",
        "Bank": "C",
        "Stock Price": 40.400001525878906
      },
      {
        "Date": "2009-11-04T00:00:00",
        "Bank": "C",
        "Stock Price": 39.70000076293945
      },
      {
        "Date": "2009-11-05T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2009-11-06T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2009-11-09T00:00:00",
        "Bank": "C",
        "Stock Price": 41.900001525878906
      },
      {
        "Date": "2009-11-10T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2009-11-11T00:00:00",
        "Bank": "C",
        "Stock Price": 41.599998474121094
      },
      {
        "Date": "2009-11-12T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {"Date": "2009-11-13T00:00:00", "Bank": "C", "Stock Price": 40.5},
      {
        "Date": "2009-11-16T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2009-11-17T00:00:00",
        "Bank": "C",
        "Stock Price": 42.400001525878906
      },
      {
        "Date": "2009-11-18T00:00:00",
        "Bank": "C",
        "Stock Price": 42.900001525878906
      },
      {
        "Date": "2009-11-19T00:00:00",
        "Bank": "C",
        "Stock Price": 42.599998474121094
      },
      {"Date": "2009-11-20T00:00:00", "Bank": "C", "Stock Price": 42},
      {
        "Date": "2009-11-23T00:00:00",
        "Bank": "C",
        "Stock Price": 42.79999923706055
      },
      {
        "Date": "2009-11-24T00:00:00",
        "Bank": "C",
        "Stock Price": 42.099998474121094
      },
      {
        "Date": "2009-11-25T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2009-11-27T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2009-11-30T00:00:00",
        "Bank": "C",
        "Stock Price": 41.099998474121094
      },
      {"Date": "2009-12-01T00:00:00", "Bank": "C", "Stock Price": 41},
      {"Date": "2009-12-02T00:00:00", "Bank": "C", "Stock Price": 41},
      {"Date": "2009-12-03T00:00:00", "Bank": "C", "Stock Price": 40.5},
      {
        "Date": "2009-12-04T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2009-12-07T00:00:00",
        "Bank": "C",
        "Stock Price": 40.29999923706055
      },
      {
        "Date": "2009-12-08T00:00:00",
        "Bank": "C",
        "Stock Price": 39.099998474121094
      },
      {
        "Date": "2009-12-09T00:00:00",
        "Bank": "C",
        "Stock Price": 38.599998474121094
      },
      {
        "Date": "2009-12-10T00:00:00",
        "Bank": "C",
        "Stock Price": 38.70000076293945
      },
      {"Date": "2009-12-11T00:00:00", "Bank": "C", "Stock Price": 39.5},
      {"Date": "2009-12-14T00:00:00", "Bank": "C", "Stock Price": 37},
      {
        "Date": "2009-12-15T00:00:00",
        "Bank": "C",
        "Stock Price": 35.599998474121094
      },
      {"Date": "2009-12-16T00:00:00", "Bank": "C", "Stock Price": 34.5},
      {"Date": "2009-12-17T00:00:00", "Bank": "C", "Stock Price": 32},
      {"Date": "2009-12-18T00:00:00", "Bank": "C", "Stock Price": 34},
      {
        "Date": "2009-12-21T00:00:00",
        "Bank": "C",
        "Stock Price": 34.20000076293945
      },
      {
        "Date": "2009-12-22T00:00:00",
        "Bank": "C",
        "Stock Price": 33.400001525878906
      },
      {
        "Date": "2009-12-23T00:00:00",
        "Bank": "C",
        "Stock Price": 32.900001525878906
      },
      {"Date": "2009-12-24T00:00:00", "Bank": "C", "Stock Price": 33.5},
      {
        "Date": "2009-12-28T00:00:00",
        "Bank": "C",
        "Stock Price": 33.900001525878906
      },
      {
        "Date": "2009-12-29T00:00:00",
        "Bank": "C",
        "Stock Price": 33.70000076293945
      },
      {
        "Date": "2009-12-30T00:00:00",
        "Bank": "C",
        "Stock Price": 33.20000076293945
      },
      {
        "Date": "2009-12-31T00:00:00",
        "Bank": "C",
        "Stock Price": 33.099998474121094
      },
      {"Date": "2010-01-04T00:00:00", "Bank": "C", "Stock Price": 34},
      {
        "Date": "2010-01-05T00:00:00",
        "Bank": "C",
        "Stock Price": 35.29999923706055
      },
      {
        "Date": "2010-01-06T00:00:00",
        "Bank": "C",
        "Stock Price": 36.400001525878906
      },
      {"Date": "2010-01-07T00:00:00", "Bank": "C", "Stock Price": 36.5},
      {
        "Date": "2010-01-08T00:00:00",
        "Bank": "C",
        "Stock Price": 35.900001525878906
      },
      {
        "Date": "2010-01-11T00:00:00",
        "Bank": "C",
        "Stock Price": 36.29999923706055
      },
      {
        "Date": "2010-01-12T00:00:00",
        "Bank": "C",
        "Stock Price": 35.20000076293945
      },
      {"Date": "2010-01-13T00:00:00", "Bank": "C", "Stock Price": 35},
      {
        "Date": "2010-01-14T00:00:00",
        "Bank": "C",
        "Stock Price": 35.099998474121094
      },
      {
        "Date": "2010-01-15T00:00:00",
        "Bank": "C",
        "Stock Price": 34.20000076293945
      },
      {
        "Date": "2010-01-19T00:00:00",
        "Bank": "C",
        "Stock Price": 35.400001525878906
      },
      {
        "Date": "2010-01-20T00:00:00",
        "Bank": "C",
        "Stock Price": 34.599998474121094
      },
      {
        "Date": "2010-01-21T00:00:00",
        "Bank": "C",
        "Stock Price": 32.70000076293945
      },
      {"Date": "2010-01-22T00:00:00", "Bank": "C", "Stock Price": 32.5},
      {
        "Date": "2010-01-25T00:00:00",
        "Bank": "C",
        "Stock Price": 32.29999923706055
      },
      {"Date": "2010-01-26T00:00:00", "Bank": "C", "Stock Price": 31.5},
      {"Date": "2010-01-27T00:00:00", "Bank": "C", "Stock Price": 32},
      {
        "Date": "2010-01-28T00:00:00",
        "Bank": "C",
        "Stock Price": 32.400001525878906
      },
      {
        "Date": "2010-01-29T00:00:00",
        "Bank": "C",
        "Stock Price": 33.20000076293945
      },
      {
        "Date": "2010-02-01T00:00:00",
        "Bank": "C",
        "Stock Price": 33.400001525878906
      },
      {
        "Date": "2010-02-02T00:00:00",
        "Bank": "C",
        "Stock Price": 34.099998474121094
      },
      {
        "Date": "2010-02-03T00:00:00",
        "Bank": "C",
        "Stock Price": 33.70000076293945
      },
      {
        "Date": "2010-02-04T00:00:00",
        "Bank": "C",
        "Stock Price": 31.799999237060547
      },
      {
        "Date": "2010-02-05T00:00:00",
        "Bank": "C",
        "Stock Price": 32.20000076293945
      },
      {"Date": "2010-02-08T00:00:00", "Bank": "C", "Stock Price": 31.5},
      {
        "Date": "2010-02-09T00:00:00",
        "Bank": "C",
        "Stock Price": 31.799999237060547
      },
      {"Date": "2010-02-10T00:00:00", "Bank": "C", "Stock Price": 32},
      {
        "Date": "2010-02-11T00:00:00",
        "Bank": "C",
        "Stock Price": 32.099998474121094
      },
      {
        "Date": "2010-02-12T00:00:00",
        "Bank": "C",
        "Stock Price": 31.799999237060547
      },
      {
        "Date": "2010-02-16T00:00:00",
        "Bank": "C",
        "Stock Price": 33.099998474121094
      },
      {
        "Date": "2010-02-17T00:00:00",
        "Bank": "C",
        "Stock Price": 34.099998474121094
      },
      {
        "Date": "2010-02-18T00:00:00",
        "Bank": "C",
        "Stock Price": 34.29999923706055
      },
      {
        "Date": "2010-02-19T00:00:00",
        "Bank": "C",
        "Stock Price": 34.20000076293945
      },
      {
        "Date": "2010-02-22T00:00:00",
        "Bank": "C",
        "Stock Price": 34.599998474121094
      },
      {"Date": "2010-02-23T00:00:00", "Bank": "C", "Stock Price": 33.5},
      {"Date": "2010-02-24T00:00:00", "Bank": "C", "Stock Price": 34.5},
      {
        "Date": "2010-02-25T00:00:00",
        "Bank": "C",
        "Stock Price": 33.900001525878906
      },
      {"Date": "2010-02-26T00:00:00", "Bank": "C", "Stock Price": 34},
      {
        "Date": "2010-03-01T00:00:00",
        "Bank": "C",
        "Stock Price": 33.900001525878906
      },
      {"Date": "2010-03-02T00:00:00", "Bank": "C", "Stock Price": 34},
      {"Date": "2010-03-03T00:00:00", "Bank": "C", "Stock Price": 34},
      {
        "Date": "2010-03-04T00:00:00",
        "Bank": "C",
        "Stock Price": 34.29999923706055
      },
      {"Date": "2010-03-05T00:00:00", "Bank": "C", "Stock Price": 35},
      {
        "Date": "2010-03-08T00:00:00",
        "Bank": "C",
        "Stock Price": 35.599998474121094
      },
      {
        "Date": "2010-03-09T00:00:00",
        "Bank": "C",
        "Stock Price": 38.20000076293945
      },
      {
        "Date": "2010-03-10T00:00:00",
        "Bank": "C",
        "Stock Price": 39.599998474121094
      },
      {
        "Date": "2010-03-11T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-03-12T00:00:00",
        "Bank": "C",
        "Stock Price": 39.70000076293945
      },
      {
        "Date": "2010-03-15T00:00:00",
        "Bank": "C",
        "Stock Price": 38.900001525878906
      },
      {"Date": "2010-03-16T00:00:00", "Bank": "C", "Stock Price": 40.5},
      {"Date": "2010-03-17T00:00:00", "Bank": "C", "Stock Price": 40.5},
      {
        "Date": "2010-03-18T00:00:00",
        "Bank": "C",
        "Stock Price": 40.20000076293945
      },
      {"Date": "2010-03-19T00:00:00", "Bank": "C", "Stock Price": 39},
      {
        "Date": "2010-03-22T00:00:00",
        "Bank": "C",
        "Stock Price": 40.400001525878906
      },
      {
        "Date": "2010-03-23T00:00:00",
        "Bank": "C",
        "Stock Price": 41.29999923706055
      },
      {"Date": "2010-03-24T00:00:00", "Bank": "C", "Stock Price": 41.5},
      {
        "Date": "2010-03-25T00:00:00",
        "Bank": "C",
        "Stock Price": 42.70000076293945
      },
      {
        "Date": "2010-03-26T00:00:00",
        "Bank": "C",
        "Stock Price": 43.099998474121094
      },
      {
        "Date": "2010-03-29T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-03-30T00:00:00",
        "Bank": "C",
        "Stock Price": 40.900001525878906
      },
      {"Date": "2010-03-31T00:00:00", "Bank": "C", "Stock Price": 40.5},
      {
        "Date": "2010-04-01T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-04-05T00:00:00",
        "Bank": "C",
        "Stock Price": 42.599998474121094
      },
      {
        "Date": "2010-04-06T00:00:00",
        "Bank": "C",
        "Stock Price": 42.900001525878906
      },
      {
        "Date": "2010-04-07T00:00:00",
        "Bank": "C",
        "Stock Price": 43.599998474121094
      },
      {
        "Date": "2010-04-08T00:00:00",
        "Bank": "C",
        "Stock Price": 44.70000076293945
      },
      {"Date": "2010-04-09T00:00:00", "Bank": "C", "Stock Price": 45.5},
      {
        "Date": "2010-04-12T00:00:00",
        "Bank": "C",
        "Stock Price": 46.400001525878906
      },
      {
        "Date": "2010-04-13T00:00:00",
        "Bank": "C",
        "Stock Price": 46.20000076293945
      },
      {
        "Date": "2010-04-14T00:00:00",
        "Bank": "C",
        "Stock Price": 49.29999923706055
      },
      {
        "Date": "2010-04-15T00:00:00",
        "Bank": "C",
        "Stock Price": 48.099998474121094
      },
      {
        "Date": "2010-04-16T00:00:00",
        "Bank": "C",
        "Stock Price": 45.599998474121094
      },
      {
        "Date": "2010-04-19T00:00:00",
        "Bank": "C",
        "Stock Price": 48.79999923706055
      },
      {
        "Date": "2010-04-20T00:00:00",
        "Bank": "C",
        "Stock Price": 49.70000076293945
      },
      {
        "Date": "2010-04-21T00:00:00",
        "Bank": "C",
        "Stock Price": 49.29999923706055
      },
      {
        "Date": "2010-04-22T00:00:00",
        "Bank": "C",
        "Stock Price": 48.70000076293945
      },
      {
        "Date": "2010-04-23T00:00:00",
        "Bank": "C",
        "Stock Price": 48.599998474121094
      },
      {
        "Date": "2010-04-26T00:00:00",
        "Bank": "C",
        "Stock Price": 46.099998474121094
      },
      {
        "Date": "2010-04-27T00:00:00",
        "Bank": "C",
        "Stock Price": 43.400001525878906
      },
      {"Date": "2010-04-28T00:00:00", "Bank": "C", "Stock Price": 44.5},
      {
        "Date": "2010-04-29T00:00:00",
        "Bank": "C",
        "Stock Price": 45.599998474121094
      },
      {
        "Date": "2010-04-30T00:00:00",
        "Bank": "C",
        "Stock Price": 43.70000076293945
      },
      {
        "Date": "2010-05-03T00:00:00",
        "Bank": "C",
        "Stock Price": 44.099998474121094
      },
      {
        "Date": "2010-05-04T00:00:00",
        "Bank": "C",
        "Stock Price": 42.599998474121094
      },
      {
        "Date": "2010-05-05T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-05-06T00:00:00",
        "Bank": "C",
        "Stock Price": 40.400001525878906
      },
      {"Date": "2010-05-07T00:00:00", "Bank": "C", "Stock Price": 40},
      {
        "Date": "2010-05-10T00:00:00",
        "Bank": "C",
        "Stock Price": 42.20000076293945
      },
      {
        "Date": "2010-05-11T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2010-05-12T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-05-13T00:00:00",
        "Bank": "C",
        "Stock Price": 40.900001525878906
      },
      {
        "Date": "2010-05-14T00:00:00",
        "Bank": "C",
        "Stock Price": 39.79999923706055
      },
      {
        "Date": "2010-05-17T00:00:00",
        "Bank": "C",
        "Stock Price": 38.599998474121094
      },
      {
        "Date": "2010-05-18T00:00:00",
        "Bank": "C",
        "Stock Price": 37.29999923706055
      },
      {
        "Date": "2010-05-19T00:00:00",
        "Bank": "C",
        "Stock Price": 38.099998474121094
      },
      {
        "Date": "2010-05-20T00:00:00",
        "Bank": "C",
        "Stock Price": 36.29999923706055
      },
      {"Date": "2010-05-21T00:00:00", "Bank": "C", "Stock Price": 37.5},
      {
        "Date": "2010-05-24T00:00:00",
        "Bank": "C",
        "Stock Price": 37.79999923706055
      },
      {
        "Date": "2010-05-25T00:00:00",
        "Bank": "C",
        "Stock Price": 37.79999923706055
      },
      {
        "Date": "2010-05-26T00:00:00",
        "Bank": "C",
        "Stock Price": 38.599998474121094
      },
      {
        "Date": "2010-05-27T00:00:00",
        "Bank": "C",
        "Stock Price": 40.20000076293945
      },
      {
        "Date": "2010-05-28T00:00:00",
        "Bank": "C",
        "Stock Price": 39.599998474121094
      },
      {"Date": "2010-06-01T00:00:00", "Bank": "C", "Stock Price": 38.5},
      {
        "Date": "2010-06-02T00:00:00",
        "Bank": "C",
        "Stock Price": 39.20000076293945
      },
      {
        "Date": "2010-06-03T00:00:00",
        "Bank": "C",
        "Stock Price": 39.599998474121094
      },
      {
        "Date": "2010-06-04T00:00:00",
        "Bank": "C",
        "Stock Price": 37.900001525878906
      },
      {
        "Date": "2010-06-07T00:00:00",
        "Bank": "C",
        "Stock Price": 36.400001525878906
      },
      {
        "Date": "2010-06-08T00:00:00",
        "Bank": "C",
        "Stock Price": 37.20000076293945
      },
      {
        "Date": "2010-06-09T00:00:00",
        "Bank": "C",
        "Stock Price": 38.70000076293945
      },
      {"Date": "2010-06-10T00:00:00", "Bank": "C", "Stock Price": 39},
      {
        "Date": "2010-06-11T00:00:00",
        "Bank": "C",
        "Stock Price": 38.79999923706055
      },
      {
        "Date": "2010-06-14T00:00:00",
        "Bank": "C",
        "Stock Price": 38.79999923706055
      },
      {
        "Date": "2010-06-15T00:00:00",
        "Bank": "C",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2010-06-16T00:00:00",
        "Bank": "C",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2010-06-17T00:00:00",
        "Bank": "C",
        "Stock Price": 39.599998474121094
      },
      {
        "Date": "2010-06-18T00:00:00",
        "Bank": "C",
        "Stock Price": 40.099998474121094
      },
      {
        "Date": "2010-06-21T00:00:00",
        "Bank": "C",
        "Stock Price": 40.20000076293945
      },
      {
        "Date": "2010-06-22T00:00:00",
        "Bank": "C",
        "Stock Price": 39.400001525878906
      },
      {
        "Date": "2010-06-23T00:00:00",
        "Bank": "C",
        "Stock Price": 38.900001525878906
      },
      {
        "Date": "2010-06-24T00:00:00",
        "Bank": "C",
        "Stock Price": 37.79999923706055
      },
      {
        "Date": "2010-06-25T00:00:00",
        "Bank": "C",
        "Stock Price": 39.400001525878906
      },
      {"Date": "2010-06-28T00:00:00", "Bank": "C", "Stock Price": 40},
      {
        "Date": "2010-06-29T00:00:00",
        "Bank": "C",
        "Stock Price": 37.29999923706055
      },
      {
        "Date": "2010-06-30T00:00:00",
        "Bank": "C",
        "Stock Price": 37.599998474121094
      },
      {
        "Date": "2010-07-01T00:00:00",
        "Bank": "C",
        "Stock Price": 37.79999923706055
      },
      {
        "Date": "2010-07-02T00:00:00",
        "Bank": "C",
        "Stock Price": 37.900001525878906
      },
      {
        "Date": "2010-07-06T00:00:00",
        "Bank": "C",
        "Stock Price": 37.900001525878906
      },
      {"Date": "2010-07-07T00:00:00", "Bank": "C", "Stock Price": 39},
      {
        "Date": "2010-07-08T00:00:00",
        "Bank": "C",
        "Stock Price": 39.70000076293945
      },
      {
        "Date": "2010-07-09T00:00:00",
        "Bank": "C",
        "Stock Price": 40.400001525878906
      },
      {
        "Date": "2010-07-12T00:00:00",
        "Bank": "C",
        "Stock Price": 41.099998474121094
      },
      {"Date": "2010-07-13T00:00:00", "Bank": "C", "Stock Price": 43},
      {
        "Date": "2010-07-14T00:00:00",
        "Bank": "C",
        "Stock Price": 42.099998474121094
      },
      {
        "Date": "2010-07-15T00:00:00",
        "Bank": "C",
        "Stock Price": 41.599998474121094
      },
      {"Date": "2010-07-16T00:00:00", "Bank": "C", "Stock Price": 39},
      {
        "Date": "2010-07-19T00:00:00",
        "Bank": "C",
        "Stock Price": 39.79999923706055
      },
      {
        "Date": "2010-07-20T00:00:00",
        "Bank": "C",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2010-07-21T00:00:00",
        "Bank": "C",
        "Stock Price": 39.400001525878906
      },
      {
        "Date": "2010-07-22T00:00:00",
        "Bank": "C",
        "Stock Price": 40.900001525878906
      },
      {
        "Date": "2010-07-23T00:00:00",
        "Bank": "C",
        "Stock Price": 40.20000076293945
      },
      {"Date": "2010-07-26T00:00:00", "Bank": "C", "Stock Price": 41.5},
      {
        "Date": "2010-07-27T00:00:00",
        "Bank": "C",
        "Stock Price": 41.599998474121094
      },
      {
        "Date": "2010-07-28T00:00:00",
        "Bank": "C",
        "Stock Price": 40.900001525878906
      },
      {
        "Date": "2010-07-29T00:00:00",
        "Bank": "C",
        "Stock Price": 41.20000076293945
      },
      {"Date": "2010-07-30T00:00:00", "Bank": "C", "Stock Price": 41},
      {
        "Date": "2010-08-02T00:00:00",
        "Bank": "C",
        "Stock Price": 41.900001525878906
      },
      {
        "Date": "2010-08-03T00:00:00",
        "Bank": "C",
        "Stock Price": 41.29999923706055
      },
      {
        "Date": "2010-08-04T00:00:00",
        "Bank": "C",
        "Stock Price": 41.400001525878906
      },
      {"Date": "2010-08-05T00:00:00", "Bank": "C", "Stock Price": 41},
      {
        "Date": "2010-08-06T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2010-08-09T00:00:00",
        "Bank": "C",
        "Stock Price": 40.79999923706055
      },
      {"Date": "2010-08-10T00:00:00", "Bank": "C", "Stock Price": 40},
      {"Date": "2010-08-11T00:00:00", "Bank": "C", "Stock Price": 38.5},
      {
        "Date": "2010-08-12T00:00:00",
        "Bank": "C",
        "Stock Price": 38.70000076293945
      },
      {
        "Date": "2010-08-13T00:00:00",
        "Bank": "C",
        "Stock Price": 38.79999923706055
      },
      {
        "Date": "2010-08-16T00:00:00",
        "Bank": "C",
        "Stock Price": 38.70000076293945
      },
      {"Date": "2010-08-17T00:00:00", "Bank": "C", "Stock Price": 38.5},
      {
        "Date": "2010-08-18T00:00:00",
        "Bank": "C",
        "Stock Price": 38.599998474121094
      },
      {
        "Date": "2010-08-19T00:00:00",
        "Bank": "C",
        "Stock Price": 37.900001525878906
      },
      {"Date": "2010-08-20T00:00:00", "Bank": "C", "Stock Price": 37.5},
      {"Date": "2010-08-23T00:00:00", "Bank": "C", "Stock Price": 37.5},
      {
        "Date": "2010-08-24T00:00:00",
        "Bank": "C",
        "Stock Price": 37.099998474121094
      },
      {
        "Date": "2010-08-25T00:00:00",
        "Bank": "C",
        "Stock Price": 36.79999923706055
      },
      {
        "Date": "2010-08-26T00:00:00",
        "Bank": "C",
        "Stock Price": 36.599998474121094
      },
      {
        "Date": "2010-08-27T00:00:00",
        "Bank": "C",
        "Stock Price": 37.599998474121094
      },
      {
        "Date": "2010-08-30T00:00:00",
        "Bank": "C",
        "Stock Price": 36.70000076293945
      },
      {
        "Date": "2010-08-31T00:00:00",
        "Bank": "C",
        "Stock Price": 37.099998474121094
      },
      {"Date": "2010-09-01T00:00:00", "Bank": "C", "Stock Price": 38.5},
      {
        "Date": "2010-09-02T00:00:00",
        "Bank": "C",
        "Stock Price": 38.79999923706055
      },
      {
        "Date": "2010-09-03T00:00:00",
        "Bank": "C",
        "Stock Price": 39.099998474121094
      },
      {
        "Date": "2010-09-07T00:00:00",
        "Bank": "C",
        "Stock Price": 38.29999923706055
      },
      {
        "Date": "2010-09-08T00:00:00",
        "Bank": "C",
        "Stock Price": 38.400001525878906
      },
      {
        "Date": "2010-09-09T00:00:00",
        "Bank": "C",
        "Stock Price": 39.099998474121094
      },
      {
        "Date": "2010-09-10T00:00:00",
        "Bank": "C",
        "Stock Price": 39.099998474121094
      },
      {
        "Date": "2010-09-13T00:00:00",
        "Bank": "C",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2010-09-14T00:00:00",
        "Bank": "C",
        "Stock Price": 39.400001525878906
      },
      {
        "Date": "2010-09-15T00:00:00",
        "Bank": "C",
        "Stock Price": 39.20000076293945
      },
      {
        "Date": "2010-09-16T00:00:00",
        "Bank": "C",
        "Stock Price": 39.70000076293945
      },
      {"Date": "2010-09-17T00:00:00", "Bank": "C", "Stock Price": 39.5},
      {
        "Date": "2010-09-20T00:00:00",
        "Bank": "C",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2010-09-21T00:00:00",
        "Bank": "C",
        "Stock Price": 39.400001525878906
      },
      {
        "Date": "2010-09-22T00:00:00",
        "Bank": "C",
        "Stock Price": 38.79999923706055
      },
      {"Date": "2010-09-23T00:00:00", "Bank": "C", "Stock Price": 38},
      {"Date": "2010-09-24T00:00:00", "Bank": "C", "Stock Price": 39},
      {
        "Date": "2010-09-27T00:00:00",
        "Bank": "C",
        "Stock Price": 38.70000076293945
      },
      {
        "Date": "2010-09-28T00:00:00",
        "Bank": "C",
        "Stock Price": 38.79999923706055
      },
      {
        "Date": "2010-09-29T00:00:00",
        "Bank": "C",
        "Stock Price": 39.20000076293945
      },
      {
        "Date": "2010-09-30T00:00:00",
        "Bank": "C",
        "Stock Price": 39.099998474121094
      },
      {
        "Date": "2010-10-01T00:00:00",
        "Bank": "C",
        "Stock Price": 40.900001525878906
      },
      {
        "Date": "2010-10-04T00:00:00",
        "Bank": "C",
        "Stock Price": 40.29999923706055
      },
      {
        "Date": "2010-10-05T00:00:00",
        "Bank": "C",
        "Stock Price": 41.29999923706055
      },
      {"Date": "2010-10-06T00:00:00", "Bank": "C", "Stock Price": 41},
      {
        "Date": "2010-10-07T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-10-08T00:00:00",
        "Bank": "C",
        "Stock Price": 41.900001525878906
      },
      {
        "Date": "2010-10-11T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-10-12T00:00:00",
        "Bank": "C",
        "Stock Price": 42.400001525878906
      },
      {"Date": "2010-10-13T00:00:00", "Bank": "C", "Stock Price": 42.5},
      {
        "Date": "2010-10-14T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {"Date": "2010-10-15T00:00:00", "Bank": "C", "Stock Price": 39.5},
      {
        "Date": "2010-10-18T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2010-10-19T00:00:00",
        "Bank": "C",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2010-10-20T00:00:00",
        "Bank": "C",
        "Stock Price": 41.099998474121094
      },
      {
        "Date": "2010-10-21T00:00:00",
        "Bank": "C",
        "Stock Price": 40.70000076293945
      },
      {
        "Date": "2010-10-22T00:00:00",
        "Bank": "C",
        "Stock Price": 41.099998474121094
      },
      {
        "Date": "2010-10-25T00:00:00",
        "Bank": "C",
        "Stock Price": 42.099998474121094
      },
      {
        "Date": "2010-10-26T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {
        "Date": "2010-10-27T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2010-10-28T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2010-10-29T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {"Date": "2010-11-01T00:00:00", "Bank": "C", "Stock Price": 41.5},
      {
        "Date": "2010-11-02T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2010-11-03T00:00:00",
        "Bank": "C",
        "Stock Price": 41.900001525878906
      },
      {
        "Date": "2010-11-04T00:00:00",
        "Bank": "C",
        "Stock Price": 43.29999923706055
      },
      {
        "Date": "2010-11-05T00:00:00",
        "Bank": "C",
        "Stock Price": 44.900001525878906
      },
      {
        "Date": "2010-11-08T00:00:00",
        "Bank": "C",
        "Stock Price": 44.400001525878906
      },
      {"Date": "2010-11-09T00:00:00", "Bank": "C", "Stock Price": 43},
      {
        "Date": "2010-11-10T00:00:00",
        "Bank": "C",
        "Stock Price": 44.20000076293945
      },
      {
        "Date": "2010-11-11T00:00:00",
        "Bank": "C",
        "Stock Price": 43.599998474121094
      },
      {
        "Date": "2010-11-12T00:00:00",
        "Bank": "C",
        "Stock Price": 42.900001525878906
      },
      {
        "Date": "2010-11-15T00:00:00",
        "Bank": "C",
        "Stock Price": 43.20000076293945
      },
      {
        "Date": "2010-11-16T00:00:00",
        "Bank": "C",
        "Stock Price": 42.20000076293945
      },
      {
        "Date": "2010-11-17T00:00:00",
        "Bank": "C",
        "Stock Price": 41.900001525878906
      },
      {"Date": "2010-11-18T00:00:00", "Bank": "C", "Stock Price": 43},
      {
        "Date": "2010-11-19T00:00:00",
        "Bank": "C",
        "Stock Price": 42.70000076293945
      },
      {
        "Date": "2010-11-22T00:00:00",
        "Bank": "C",
        "Stock Price": 41.79999923706055
      },
      {"Date": "2010-11-23T00:00:00", "Bank": "C", "Stock Price": 41},
      {
        "Date": "2010-11-24T00:00:00",
        "Bank": "C",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2010-11-26T00:00:00",
        "Bank": "C",
        "Stock Price": 41.099998474121094
      },
      {"Date": "2010-11-29T00:00:00", "Bank": "C", "Stock Price": 41.5},
      {"Date": "2010-11-30T00:00:00", "Bank": "C", "Stock Price": 42},
      {"Date": "2010-12-01T00:00:00", "Bank": "C", "Stock Price": 43},
      {
        "Date": "2010-12-02T00:00:00",
        "Bank": "C",
        "Stock Price": 44.20000076293945
      },
      {"Date": "2010-12-03T00:00:00", "Bank": "C", "Stock Price": 44.5},
      {"Date": "2010-12-06T00:00:00", "Bank": "C", "Stock Price": 44.5},
      {
        "Date": "2010-12-07T00:00:00",
        "Bank": "C",
        "Stock Price": 46.20000076293945
      },
      {
        "Date": "2010-12-08T00:00:00",
        "Bank": "C",
        "Stock Price": 46.400001525878906
      },
      {
        "Date": "2010-12-09T00:00:00",
        "Bank": "C",
        "Stock Price": 46.900001525878906
      },
      {
        "Date": "2010-12-10T00:00:00",
        "Bank": "C",
        "Stock Price": 47.70000076293945
      },
      {
        "Date": "2010-12-13T00:00:00",
        "Bank": "C",
        "Stock Price": 48.099998474121094
      },
      {
        "Date": "2010-12-14T00:00:00",
        "Bank": "C",
        "Stock Price": 46.900001525878906
      },
      {
        "Date": "2010-12-15T00:00:00",
        "Bank": "C",
        "Stock Price": 45.900001525878906
      },
      {
        "Date": "2010-12-16T00:00:00",
        "Bank": "C",
        "Stock Price": 45.900001525878906
      },
      {"Date": "2010-12-17T00:00:00", "Bank": "C", "Stock Price": 47},
      {
        "Date": "2010-12-20T00:00:00",
        "Bank": "C",
        "Stock Price": 47.099998474121094
      },
      {
        "Date": "2010-12-21T00:00:00",
        "Bank": "C",
        "Stock Price": 47.400001525878906
      },
      {
        "Date": "2010-12-22T00:00:00",
        "Bank": "C",
        "Stock Price": 47.29999923706055
      },
      {
        "Date": "2010-12-23T00:00:00",
        "Bank": "C",
        "Stock Price": 46.79999923706055
      },
      {
        "Date": "2010-12-27T00:00:00",
        "Bank": "C",
        "Stock Price": 47.70000076293945
      },
      {
        "Date": "2010-12-28T00:00:00",
        "Bank": "C",
        "Stock Price": 47.79999923706055
      },
      {
        "Date": "2010-12-29T00:00:00",
        "Bank": "C",
        "Stock Price": 47.70000076293945
      },
      {
        "Date": "2010-12-30T00:00:00",
        "Bank": "C",
        "Stock Price": 47.599998474121094
      },
      {
        "Date": "2007-01-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 200.72000122070312
      },
      {
        "Date": "2007-01-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 198.85000610351562
      },
      {
        "Date": "2007-01-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.0500030517578
      },
      {
        "Date": "2007-01-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 203.72999572753906
      },
      {
        "Date": "2007-01-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 204.0800018310547
      },
      {
        "Date": "2007-01-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 208.11000061035156
      },
      {
        "Date": "2007-01-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.8800048828125
      },
      {
        "Date": "2007-01-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.99000549316406
      },
      {
        "Date": "2007-01-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.58999633789062
      },
      {
        "Date": "2007-01-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.22999572753906
      },
      {
        "Date": "2007-01-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 209.67999267578125
      },
      {
        "Date": "2007-01-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 210.2899932861328
      },
      {
        "Date": "2007-01-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 212.97000122070312
      },
      {
        "Date": "2007-01-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 212.63999938964844
      },
      {
        "Date": "2007-01-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.10000610351562
      },
      {
        "Date": "2007-01-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.07000732421875
      },
      {"Date": "2007-01-26T00:00:00", "Bank": "GS", "Stock Price": 213.5},
      {
        "Date": "2007-01-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.0399932861328
      },
      {
        "Date": "2007-01-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 208.77999877929688
      },
      {
        "Date": "2007-01-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 212.16000366210938
      },
      {"Date": "2007-02-01T00:00:00", "Bank": "GS", "Stock Price": 212},
      {
        "Date": "2007-02-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.42999267578125
      },
      {
        "Date": "2007-02-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 212.5500030517578
      },
      {
        "Date": "2007-02-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.64999389648438
      },
      {
        "Date": "2007-02-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.5500030517578
      },
      {
        "Date": "2007-02-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.89999389648438
      },
      {
        "Date": "2007-02-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.27999877929688
      },
      {
        "Date": "2007-02-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.1300048828125
      },
      {
        "Date": "2007-02-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 212.52999877929688
      },
      {
        "Date": "2007-02-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 217.39999389648438
      },
      {
        "Date": "2007-02-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.82000732421875
      },
      {
        "Date": "2007-02-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.9199981689453
      },
      {
        "Date": "2007-02-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.94000244140625
      },
      {
        "Date": "2007-02-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.14999389648438
      },
      {
        "Date": "2007-02-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 218.97000122070312
      },
      {"Date": "2007-02-23T00:00:00", "Bank": "GS", "Stock Price": 216.5},
      {"Date": "2007-02-26T00:00:00", "Bank": "GS", "Stock Price": 214},
      {"Date": "2007-02-27T00:00:00", "Bank": "GS", "Stock Price": 196},
      {"Date": "2007-02-28T00:00:00", "Bank": "GS", "Stock Price": 201.75},
      {
        "Date": "2007-03-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.66000366210938
      },
      {
        "Date": "2007-03-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 195.6699981689453
      },
      {"Date": "2007-03-05T00:00:00", "Bank": "GS", "Stock Price": 190},
      {
        "Date": "2007-03-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 197.3699951171875
      },
      {
        "Date": "2007-03-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 195.58999633789062
      },
      {
        "Date": "2007-03-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.94000244140625
      },
      {
        "Date": "2007-03-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 201.6999969482422
      },
      {
        "Date": "2007-03-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 202.60000610351562
      },
      {
        "Date": "2007-03-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.02999877929688
      },
      {
        "Date": "2007-03-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 200.14999389648438
      },
      {
        "Date": "2007-03-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 200.88999938964844
      },
      {"Date": "2007-03-16T00:00:00", "Bank": "GS", "Stock Price": 199},
      {
        "Date": "2007-03-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 202.44000244140625
      },
      {"Date": "2007-03-20T00:00:00", "Bank": "GS", "Stock Price": 204},
      {
        "Date": "2007-03-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 210.9499969482422
      },
      {
        "Date": "2007-03-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 210.0800018310547
      },
      {
        "Date": "2007-03-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.88999938964844
      },
      {
        "Date": "2007-03-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.72999572753906
      },
      {
        "Date": "2007-03-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 209.8699951171875
      },
      {
        "Date": "2007-03-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 206.75999450683594
      },
      {
        "Date": "2007-03-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 207.1999969482422
      },
      {
        "Date": "2007-03-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 206.6300048828125
      },
      {
        "Date": "2007-04-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 205.64999389648438
      },
      {"Date": "2007-04-03T00:00:00", "Bank": "GS", "Stock Price": 209.75},
      {
        "Date": "2007-04-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 208.7899932861328
      },
      {
        "Date": "2007-04-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 207.92999267578125
      },
      {
        "Date": "2007-04-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 208.94000244140625
      },
      {
        "Date": "2007-04-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 209.0500030517578
      },
      {
        "Date": "2007-04-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 206.92999267578125
      },
      {
        "Date": "2007-04-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 207.0500030517578
      },
      {"Date": "2007-04-13T00:00:00", "Bank": "GS", "Stock Price": 206.5},
      {
        "Date": "2007-04-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.52000427246094
      },
      {
        "Date": "2007-04-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.89999389648438
      },
      {"Date": "2007-04-18T00:00:00", "Bank": "GS", "Stock Price": 216.75},
      {
        "Date": "2007-04-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 219.2899932861328
      },
      {"Date": "2007-04-20T00:00:00", "Bank": "GS", "Stock Price": 220},
      {
        "Date": "2007-04-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 222.4199981689453
      },
      {
        "Date": "2007-04-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.72000122070312
      },
      {
        "Date": "2007-04-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 225.60000610351562
      },
      {
        "Date": "2007-04-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.80999755859375
      },
      {
        "Date": "2007-04-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.27999877929688
      },
      {
        "Date": "2007-04-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 218.61000061035156
      },
      {
        "Date": "2007-05-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 218.5800018310547
      },
      {
        "Date": "2007-05-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 219.49000549316406
      },
      {
        "Date": "2007-05-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 221.55999755859375
      },
      {
        "Date": "2007-05-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.33999633789062
      },
      {
        "Date": "2007-05-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.22000122070312
      },
      {
        "Date": "2007-05-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.9499969482422
      },
      {
        "Date": "2007-05-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.57000732421875
      },
      {
        "Date": "2007-05-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 223.10000610351562
      },
      {"Date": "2007-05-11T00:00:00", "Bank": "GS", "Stock Price": 227.5},
      {
        "Date": "2007-05-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.17999267578125
      },
      {
        "Date": "2007-05-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.3800048828125
      },
      {
        "Date": "2007-05-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.11000061035156
      },
      {
        "Date": "2007-05-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.3800048828125
      },
      {
        "Date": "2007-05-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 230.33999633789062
      },
      {
        "Date": "2007-05-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 229.22999572753906
      },
      {
        "Date": "2007-05-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 230.7100067138672
      },
      {
        "Date": "2007-05-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 228.5399932861328
      },
      {
        "Date": "2007-05-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 225.67999267578125
      },
      {
        "Date": "2007-05-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 225.52999877929688
      },
      {
        "Date": "2007-05-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 228.44000244140625
      },
      {"Date": "2007-05-30T00:00:00", "Bank": "GS", "Stock Price": 232},
      {
        "Date": "2007-05-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 230.82000732421875
      },
      {
        "Date": "2007-06-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 230.7100067138672
      },
      {
        "Date": "2007-06-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 229.7100067138672
      },
      {
        "Date": "2007-06-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 229.36000061035156
      },
      {
        "Date": "2007-06-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.35000610351562
      },
      {
        "Date": "2007-06-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.0500030517578
      },
      {
        "Date": "2007-06-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 225.05999755859375
      },
      {
        "Date": "2007-06-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.16000366210938
      },
      {
        "Date": "2007-06-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.85000610351562
      },
      {
        "Date": "2007-06-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 233.63999938964844
      },
      {"Date": "2007-06-14T00:00:00", "Bank": "GS", "Stock Price": 225.75},
      {
        "Date": "2007-06-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.19000244140625
      },
      {
        "Date": "2007-06-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.97000122070312
      },
      {
        "Date": "2007-06-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 229.47000122070312
      },
      {
        "Date": "2007-06-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 225.88999938964844
      },
      {
        "Date": "2007-06-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.89999389648438
      },
      {
        "Date": "2007-06-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 222.39999389648438
      },
      {
        "Date": "2007-06-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.74000549316406
      },
      {
        "Date": "2007-06-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.1699981689453
      },
      {
        "Date": "2007-06-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 219.3300018310547
      },
      {
        "Date": "2007-06-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 218.9600067138672
      },
      {"Date": "2007-06-29T00:00:00", "Bank": "GS", "Stock Price": 216.75},
      {
        "Date": "2007-07-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 219.17999267578125
      },
      {
        "Date": "2007-07-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.5500030517578
      },
      {
        "Date": "2007-07-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 221.32000732421875
      },
      {
        "Date": "2007-07-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 223.63999938964844
      },
      {
        "Date": "2007-07-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 223.3000030517578
      },
      {
        "Date": "2007-07-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 217.0800018310547
      },
      {
        "Date": "2007-07-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.72000122070312
      },
      {
        "Date": "2007-07-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.2899932861328
      },
      {
        "Date": "2007-07-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 222.17999267578125
      },
      {
        "Date": "2007-07-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.39999389648438
      },
      {
        "Date": "2007-07-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 219.39999389648438
      },
      {
        "Date": "2007-07-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.99000549316406
      },
      {
        "Date": "2007-07-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.69000244140625
      },
      {
        "Date": "2007-07-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 205.94000244140625
      },
      {
        "Date": "2007-07-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 205.0399932861328
      },
      {
        "Date": "2007-07-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 198.14999389648438
      },
      {
        "Date": "2007-07-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 203.16000366210938
      },
      {
        "Date": "2007-07-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 195.1199951171875
      },
      {
        "Date": "2007-07-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 192.64999389648438
      },
      {
        "Date": "2007-07-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 195.74000549316406
      },
      {
        "Date": "2007-07-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.33999633789062
      },
      {"Date": "2007-08-01T00:00:00", "Bank": "GS", "Stock Price": 189},
      {
        "Date": "2007-08-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.4600067138672
      },
      {
        "Date": "2007-08-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.67999267578125
      },
      {
        "Date": "2007-08-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.7899932861328
      },
      {"Date": "2007-08-07T00:00:00", "Bank": "GS", "Stock Price": 191.25},
      {
        "Date": "2007-08-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 193.3000030517578
      },
      {"Date": "2007-08-09T00:00:00", "Bank": "GS", "Stock Price": 182.25},
      {"Date": "2007-08-10T00:00:00", "Bank": "GS", "Stock Price": 180.5},
      {"Date": "2007-08-13T00:00:00", "Bank": "GS", "Stock Price": 177.5},
      {"Date": "2007-08-14T00:00:00", "Bank": "GS", "Stock Price": 169.75},
      {
        "Date": "2007-08-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.89999389648438
      },
      {
        "Date": "2007-08-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.85000610351562
      },
      {"Date": "2007-08-17T00:00:00", "Bank": "GS", "Stock Price": 175},
      {
        "Date": "2007-08-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.75999450683594
      },
      {
        "Date": "2007-08-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 175.47999572753906
      },
      {
        "Date": "2007-08-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.88999938964844
      },
      {"Date": "2007-08-23T00:00:00", "Bank": "GS", "Stock Price": 177.5},
      {
        "Date": "2007-08-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.72999572753906
      },
      {
        "Date": "2007-08-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.9499969482422
      },
      {
        "Date": "2007-08-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.9499969482422
      },
      {
        "Date": "2007-08-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.72000122070312
      },
      {
        "Date": "2007-08-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.3800048828125
      },
      {
        "Date": "2007-08-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.00999450683594
      },
      {
        "Date": "2007-09-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.8000030517578
      },
      {
        "Date": "2007-09-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.80999755859375
      },
      {
        "Date": "2007-09-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.17999267578125
      },
      {
        "Date": "2007-09-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.97999572753906
      },
      {
        "Date": "2007-09-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.61000061035156
      },
      {"Date": "2007-09-11T00:00:00", "Bank": "GS", "Stock Price": 183.5},
      {
        "Date": "2007-09-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 182.52999877929688
      },
      {
        "Date": "2007-09-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.47000122070312
      },
      {
        "Date": "2007-09-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.58999633789062
      },
      {
        "Date": "2007-09-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.61000061035156
      },
      {"Date": "2007-09-18T00:00:00", "Bank": "GS", "Stock Price": 200.5},
      {"Date": "2007-09-19T00:00:00", "Bank": "GS", "Stock Price": 205.5},
      {
        "Date": "2007-09-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 203.52999877929688
      },
      {
        "Date": "2007-09-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 209.97999572753906
      },
      {
        "Date": "2007-09-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 210.42999267578125
      },
      {
        "Date": "2007-09-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 210.89999389648438
      },
      {
        "Date": "2007-09-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.61000061035156
      },
      {
        "Date": "2007-09-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.77999877929688
      },
      {
        "Date": "2007-09-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.74000549316406
      },
      {
        "Date": "2007-10-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 222.97999572753906
      },
      {
        "Date": "2007-10-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 228.02000427246094
      },
      {
        "Date": "2007-10-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.35000610351562
      },
      {
        "Date": "2007-10-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 225.9499969482422
      },
      {"Date": "2007-10-05T00:00:00", "Bank": "GS", "Stock Price": 228.5},
      {
        "Date": "2007-10-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.9600067138672
      },
      {
        "Date": "2007-10-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 239.1999969482422
      },
      {
        "Date": "2007-10-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 235.94000244140625
      },
      {
        "Date": "2007-10-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 229.00999450683594
      },
      {
        "Date": "2007-10-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 233.55999755859375
      },
      {
        "Date": "2007-10-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 229.33999633789062
      },
      {
        "Date": "2007-10-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.8300018310547
      },
      {
        "Date": "2007-10-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.6199951171875
      },
      {
        "Date": "2007-10-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.85000610351562
      },
      {
        "Date": "2007-10-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 217.69000244140625
      },
      {
        "Date": "2007-10-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 222.17999267578125
      },
      {
        "Date": "2007-10-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 223.75999450683594
      },
      {
        "Date": "2007-10-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 225.1199951171875
      },
      {
        "Date": "2007-10-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.66000366210938
      },
      {
        "Date": "2007-10-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 235.9199981689453
      },
      {
        "Date": "2007-10-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 243.80999755859375
      },
      {
        "Date": "2007-10-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 240.3300018310547
      },
      {
        "Date": "2007-10-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 247.9199981689453
      },
      {
        "Date": "2007-11-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 240.2100067138672
      },
      {
        "Date": "2007-11-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 229.60000610351562
      },
      {
        "Date": "2007-11-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 218.38999938964844
      },
      {
        "Date": "2007-11-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 223.16000366210938
      },
      {
        "Date": "2007-11-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.17999267578125
      },
      {
        "Date": "2007-11-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 209.94000244140625
      },
      {
        "Date": "2007-11-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.3300018310547
      },
      {
        "Date": "2007-11-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.7100067138672
      },
      {
        "Date": "2007-11-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 233.0399932861328
      },
      {
        "Date": "2007-11-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 233.30999755859375
      },
      {
        "Date": "2007-11-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.02000427246094
      },
      {"Date": "2007-11-16T00:00:00", "Bank": "GS", "Stock Price": 225.25},
      {
        "Date": "2007-11-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 220.5399932861328
      },
      {
        "Date": "2007-11-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 217.47999572753906
      },
      {"Date": "2007-11-21T00:00:00", "Bank": "GS", "Stock Price": 209.5},
      {
        "Date": "2007-11-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.47999572753906
      },
      {
        "Date": "2007-11-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 207.4499969482422
      },
      {
        "Date": "2007-11-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 213.3300018310547
      },
      {
        "Date": "2007-11-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 227.52000427246094
      },
      {
        "Date": "2007-11-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.3800048828125
      },
      {
        "Date": "2007-11-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.63999938964844
      },
      {
        "Date": "2007-12-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 226.88999938964844
      },
      {
        "Date": "2007-12-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 215.22000122070312
      },
      {
        "Date": "2007-12-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 218.25999450683594
      },
      {
        "Date": "2007-12-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 222.50999450683594
      },
      {
        "Date": "2007-12-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 217.88999938964844
      },
      {
        "Date": "2007-12-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 224.2100067138672
      },
      {
        "Date": "2007-12-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.14999389648438
      },
      {
        "Date": "2007-12-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 212.5800018310547
      },
      {
        "Date": "2007-12-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 208.47999572753906
      },
      {
        "Date": "2007-12-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 210.6699981689453
      },
      {
        "Date": "2007-12-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 208.6300048828125
      },
      {
        "Date": "2007-12-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 201.50999450683594
      },
      {
        "Date": "2007-12-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 204.16000366210938
      },
      {
        "Date": "2007-12-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 202.6699981689453
      },
      {
        "Date": "2007-12-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 209.60000610351562
      },
      {
        "Date": "2007-12-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 214.32000732421875
      },
      {
        "Date": "2007-12-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 216.69000244140625
      },
      {
        "Date": "2007-12-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.9499969482422
      },
      {
        "Date": "2007-12-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 211.94000244140625
      },
      {
        "Date": "2007-12-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 215.0500030517578
      },
      {
        "Date": "2008-01-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 207.60000610351562
      },
      {
        "Date": "2008-01-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 204.83999633789062
      },
      {
        "Date": "2008-01-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.92999267578125
      },
      {
        "Date": "2008-01-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 194.72999572753906
      },
      {"Date": "2008-01-08T00:00:00", "Bank": "GS", "Stock Price": 189.5},
      {"Date": "2008-01-09T00:00:00", "Bank": "GS", "Stock Price": 191.75},
      {
        "Date": "2008-01-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 196.91000366210938
      },
      {
        "Date": "2008-01-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 198.74000549316406
      },
      {
        "Date": "2008-01-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 201.64999389648438
      },
      {
        "Date": "2008-01-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 193.2899932861328
      },
      {"Date": "2008-01-16T00:00:00", "Bank": "GS", "Stock Price": 197.5},
      {
        "Date": "2008-01-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.97999572753906
      },
      {
        "Date": "2008-01-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.2100067138672
      },
      {
        "Date": "2008-01-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.69000244140625
      },
      {
        "Date": "2008-01-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.38999938964844
      },
      {
        "Date": "2008-01-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.1999969482422
      },
      {
        "Date": "2008-01-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 191.3699951171875
      },
      {"Date": "2008-01-28T00:00:00", "Bank": "GS", "Stock Price": 196.25},
      {
        "Date": "2008-01-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 196.0500030517578
      },
      {
        "Date": "2008-01-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 198.5500030517578
      },
      {
        "Date": "2008-01-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.5500030517578
      },
      {
        "Date": "2008-02-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 207.77999877929688
      },
      {
        "Date": "2008-02-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 200.8000030517578
      },
      {
        "Date": "2008-02-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 189.86000061035156
      },
      {
        "Date": "2008-02-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.1699981689453
      },
      {
        "Date": "2008-02-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.4600067138672
      },
      {
        "Date": "2008-02-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.07000732421875
      },
      {
        "Date": "2008-02-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 185.8699951171875
      },
      {
        "Date": "2008-02-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.64999389648438
      },
      {
        "Date": "2008-02-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.17999267578125
      },
      {
        "Date": "2008-02-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.55999755859375
      },
      {
        "Date": "2008-02-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.41000366210938
      },
      {
        "Date": "2008-02-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.8000030517578
      },
      {"Date": "2008-02-20T00:00:00", "Bank": "GS", "Stock Price": 177.25},
      {
        "Date": "2008-02-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 175.1699981689453
      },
      {
        "Date": "2008-02-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.7100067138672
      },
      {
        "Date": "2008-02-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.36000061035156
      },
      {
        "Date": "2008-02-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.6999969482422
      },
      {
        "Date": "2008-02-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.8000030517578
      },
      {
        "Date": "2008-02-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.6999969482422
      },
      {
        "Date": "2008-02-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.6300048828125
      },
      {
        "Date": "2008-03-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.0800018310547
      },
      {
        "Date": "2008-03-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.60000610351562
      },
      {
        "Date": "2008-03-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.97000122070312
      },
      {
        "Date": "2008-03-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.64999389648438
      },
      {
        "Date": "2008-03-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.07000732421875
      },
      {
        "Date": "2008-03-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.5800018310547
      },
      {
        "Date": "2008-03-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.07000732421875
      },
      {
        "Date": "2008-03-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.00999450683594
      },
      {
        "Date": "2008-03-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.44000244140625
      },
      {
        "Date": "2008-03-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.86000061035156
      },
      {
        "Date": "2008-03-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 151.02000427246094
      },
      {
        "Date": "2008-03-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 175.58999633789062
      },
      {
        "Date": "2008-03-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.49000549316406
      },
      {
        "Date": "2008-03-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.6300048828125
      },
      {
        "Date": "2008-03-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.8800048828125
      },
      {
        "Date": "2008-03-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.6300048828125
      },
      {
        "Date": "2008-03-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 175.47999572753906
      },
      {
        "Date": "2008-03-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.13999938964844
      },
      {
        "Date": "2008-03-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.4499969482422
      },
      {
        "Date": "2008-03-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.38999938964844
      },
      {
        "Date": "2008-04-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.86000061035156
      },
      {
        "Date": "2008-04-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.8699951171875
      },
      {
        "Date": "2008-04-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.52999877929688
      },
      {
        "Date": "2008-04-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 175.39999389648438
      },
      {
        "Date": "2008-04-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.72999572753906
      },
      {
        "Date": "2008-04-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.89999389648438
      },
      {
        "Date": "2008-04-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.13999938964844
      },
      {
        "Date": "2008-04-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.5500030517578
      },
      {
        "Date": "2008-04-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.3000030517578
      },
      {
        "Date": "2008-04-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.58999633789062
      },
      {
        "Date": "2008-04-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.1999969482422
      },
      {
        "Date": "2008-04-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.0500030517578
      },
      {
        "Date": "2008-04-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.10000610351562
      },
      {
        "Date": "2008-04-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.92999267578125
      },
      {
        "Date": "2008-04-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.39999389648438
      },
      {
        "Date": "2008-04-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.75999450683594
      },
      {
        "Date": "2008-04-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.35000610351562
      },
      {
        "Date": "2008-04-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.7899932861328
      },
      {"Date": "2008-04-25T00:00:00", "Bank": "GS", "Stock Price": 192},
      {
        "Date": "2008-04-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.24000549316406
      },
      {
        "Date": "2008-04-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 192.67999267578125
      },
      {
        "Date": "2008-04-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 191.3699951171875
      },
      {
        "Date": "2008-05-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 199.0500030517578
      },
      {
        "Date": "2008-05-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 200.27000427246094
      },
      {
        "Date": "2008-05-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 197.1199951171875
      },
      {
        "Date": "2008-05-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 197.61000061035156
      },
      {
        "Date": "2008-05-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 189.75999450683594
      },
      {
        "Date": "2008-05-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.72000122070312
      },
      {
        "Date": "2008-05-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.08999633789062
      },
      {
        "Date": "2008-05-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 192.0800018310547
      },
      {
        "Date": "2008-05-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.3300018310547
      },
      {
        "Date": "2008-05-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.1300048828125
      },
      {
        "Date": "2008-05-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.6199951171875
      },
      {
        "Date": "2008-05-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.13999938964844
      },
      {
        "Date": "2008-05-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 184.39999389648438
      },
      {
        "Date": "2008-05-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 182.42999267578125
      },
      {
        "Date": "2008-05-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.60000610351562
      },
      {
        "Date": "2008-05-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.1999969482422
      },
      {
        "Date": "2008-05-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.63999938964844
      },
      {
        "Date": "2008-05-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.9199981689453
      },
      {
        "Date": "2008-05-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.8300018310547
      },
      {
        "Date": "2008-05-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.24000549316406
      },
      {
        "Date": "2008-05-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.41000366210938
      },
      {
        "Date": "2008-06-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.33999633789062
      },
      {
        "Date": "2008-06-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.5800018310547
      },
      {
        "Date": "2008-06-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.10000610351562
      },
      {
        "Date": "2008-06-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.60000610351562
      },
      {
        "Date": "2008-06-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.44000244140625
      },
      {
        "Date": "2008-06-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.75999450683594
      },
      {
        "Date": "2008-06-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.2100067138672
      },
      {
        "Date": "2008-06-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.39999389648438
      },
      {"Date": "2008-06-12T00:00:00", "Bank": "GS", "Stock Price": 166.75},
      {
        "Date": "2008-06-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.2899932861328
      },
      {
        "Date": "2008-06-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 182.08999633789062
      },
      {
        "Date": "2008-06-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.44000244140625
      },
      {
        "Date": "2008-06-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 182.77000427246094
      },
      {
        "Date": "2008-06-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 186.92999267578125
      },
      {
        "Date": "2008-06-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.77000427246094
      },
      {
        "Date": "2008-06-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.58999633789062
      },
      {
        "Date": "2008-06-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 181.97999572753906
      },
      {
        "Date": "2008-06-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.64999389648438
      },
      {
        "Date": "2008-06-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.25999450683594
      },
      {
        "Date": "2008-06-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.55999755859375
      },
      {
        "Date": "2008-06-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.89999389648438
      },
      {
        "Date": "2008-07-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 175.3300018310547
      },
      {
        "Date": "2008-07-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.7899932861328
      },
      {
        "Date": "2008-07-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.88999938964844
      },
      {
        "Date": "2008-07-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.82000732421875
      },
      {
        "Date": "2008-07-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.89999389648438
      },
      {
        "Date": "2008-07-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.02000427246094
      },
      {
        "Date": "2008-07-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.16000366210938
      },
      {
        "Date": "2008-07-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.47999572753906
      },
      {
        "Date": "2008-07-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.6699981689453
      },
      {
        "Date": "2008-07-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.8000030517578
      },
      {
        "Date": "2008-07-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.86000061035156
      },
      {
        "Date": "2008-07-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 181.24000549316406
      },
      {
        "Date": "2008-07-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 182.83999633789062
      },
      {
        "Date": "2008-07-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.77999877929688
      },
      {
        "Date": "2008-07-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.0399932861328
      },
      {
        "Date": "2008-07-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.8699951171875
      },
      {
        "Date": "2008-07-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.25999450683594
      },
      {
        "Date": "2008-07-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.66000366210938
      },
      {
        "Date": "2008-07-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.89999389648438
      },
      {
        "Date": "2008-07-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 181.6300048828125
      },
      {
        "Date": "2008-07-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 186.1699981689453
      },
      {
        "Date": "2008-07-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 184.0399932861328
      },
      {"Date": "2008-08-01T00:00:00", "Bank": "GS", "Stock Price": 182},
      {
        "Date": "2008-08-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.86000061035156
      },
      {
        "Date": "2008-08-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.77000427246094
      },
      {
        "Date": "2008-08-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.5500030517578
      },
      {
        "Date": "2008-08-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.3300018310547
      },
      {
        "Date": "2008-08-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 175.9499969482422
      },
      {"Date": "2008-08-11T00:00:00", "Bank": "GS", "Stock Price": 178},
      {
        "Date": "2008-08-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.3000030517578
      },
      {
        "Date": "2008-08-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.89999389648438
      },
      {
        "Date": "2008-08-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.58999633789062
      },
      {
        "Date": "2008-08-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.17999267578125
      },
      {
        "Date": "2008-08-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.0399932861328
      },
      {"Date": "2008-08-19T00:00:00", "Bank": "GS", "Stock Price": 158},
      {"Date": "2008-08-20T00:00:00", "Bank": "GS", "Stock Price": 158.25},
      {
        "Date": "2008-08-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.4199981689453
      },
      {
        "Date": "2008-08-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.80999755859375
      },
      {
        "Date": "2008-08-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.7100067138672
      },
      {
        "Date": "2008-08-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.91000366210938
      },
      {
        "Date": "2008-08-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.47999572753906
      },
      {
        "Date": "2008-08-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.8300018310547
      },
      {
        "Date": "2008-08-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.97000122070312
      },
      {
        "Date": "2008-09-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.32000732421875
      },
      {
        "Date": "2008-09-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.61000061035156
      },
      {
        "Date": "2008-09-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.89999389648438
      },
      {
        "Date": "2008-09-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.24000549316406
      },
      {
        "Date": "2008-09-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.72999572753906
      },
      {
        "Date": "2008-09-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.6699981689453
      },
      {
        "Date": "2008-09-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.58999633789062
      },
      {
        "Date": "2008-09-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.02999877929688
      },
      {
        "Date": "2008-09-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 154.2100067138672
      },
      {"Date": "2008-09-15T00:00:00", "Bank": "GS", "Stock Price": 135.5},
      {
        "Date": "2008-09-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 133.00999450683594
      },
      {"Date": "2008-09-17T00:00:00", "Bank": "GS", "Stock Price": 114.5},
      {"Date": "2008-09-18T00:00:00", "Bank": "GS", "Stock Price": 108},
      {
        "Date": "2008-09-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 129.8000030517578
      },
      {
        "Date": "2008-09-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 120.77999877929688
      },
      {
        "Date": "2008-09-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 125.05000305175781
      },
      {"Date": "2008-09-24T00:00:00", "Bank": "GS", "Stock Price": 133},
      {"Date": "2008-09-25T00:00:00", "Bank": "GS", "Stock Price": 135.5},
      {
        "Date": "2008-09-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.99000549316406
      },
      {
        "Date": "2008-09-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 120.69999694824219
      },
      {"Date": "2008-09-30T00:00:00", "Bank": "GS", "Stock Price": 128},
      {"Date": "2008-10-01T00:00:00", "Bank": "GS", "Stock Price": 134.5},
      {
        "Date": "2008-10-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 131.5399932861328
      },
      {"Date": "2008-10-03T00:00:00", "Bank": "GS", "Stock Price": 128},
      {"Date": "2008-10-06T00:00:00", "Bank": "GS", "Stock Price": 124},
      {"Date": "2008-10-07T00:00:00", "Bank": "GS", "Stock Price": 115},
      {"Date": "2008-10-08T00:00:00", "Bank": "GS", "Stock Price": 113},
      {
        "Date": "2008-10-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 101.3499984741211
      },
      {
        "Date": "2008-10-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 88.80000305175781
      },
      {"Date": "2008-10-13T00:00:00", "Bank": "GS", "Stock Price": 111},
      {
        "Date": "2008-10-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 122.9000015258789
      },
      {
        "Date": "2008-10-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 113.1500015258789
      },
      {
        "Date": "2008-10-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 112.4000015258789
      },
      {
        "Date": "2008-10-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 114.30000305175781
      },
      {"Date": "2008-10-20T00:00:00", "Bank": "GS", "Stock Price": 121.5},
      {
        "Date": "2008-10-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 121.3499984741211
      },
      {
        "Date": "2008-10-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 115.05999755859375
      },
      {
        "Date": "2008-10-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 108.58000183105469
      },
      {
        "Date": "2008-10-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 100.4000015258789
      },
      {
        "Date": "2008-10-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 92.87999725341797
      },
      {
        "Date": "2008-10-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 93.56999969482422
      },
      {
        "Date": "2008-10-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 97.66000366210938
      },
      {
        "Date": "2008-10-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 91.11000061035156
      },
      {"Date": "2008-10-31T00:00:00", "Bank": "GS", "Stock Price": 92.5},
      {
        "Date": "2008-11-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 89.08999633789062
      },
      {"Date": "2008-11-04T00:00:00", "Bank": "GS", "Stock Price": 95},
      {
        "Date": "2008-11-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 87.43000030517578
      },
      {
        "Date": "2008-11-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 80.72000122070312
      },
      {
        "Date": "2008-11-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 77.77999877929688
      },
      {
        "Date": "2008-11-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 71.20999908447266
      },
      {
        "Date": "2008-11-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 74.68000030517578
      },
      {
        "Date": "2008-11-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 66.79000091552734
      },
      {
        "Date": "2008-11-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 69.98999786376953
      },
      {
        "Date": "2008-11-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 66.7300033569336
      },
      {
        "Date": "2008-11-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 62.4900016784668
      },
      {
        "Date": "2008-11-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 62.029998779296875
      },
      {
        "Date": "2008-11-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 55.18000030517578
      },
      {"Date": "2008-11-20T00:00:00", "Bank": "GS", "Stock Price": 52},
      {
        "Date": "2008-11-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 53.310001373291016
      },
      {
        "Date": "2008-11-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 67.41999816894531
      },
      {
        "Date": "2008-11-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 71.77999877929688
      },
      {"Date": "2008-11-26T00:00:00", "Bank": "GS", "Stock Price": 76.5},
      {
        "Date": "2008-11-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 78.98999786376953
      },
      {
        "Date": "2008-12-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 65.76000213623047
      },
      {"Date": "2008-12-02T00:00:00", "Bank": "GS", "Stock Price": 65},
      {
        "Date": "2008-12-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 68.94999694824219
      },
      {
        "Date": "2008-12-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 67.52999877929688
      },
      {
        "Date": "2008-12-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 70.72000122070312
      },
      {
        "Date": "2008-12-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 77.1500015258789
      },
      {
        "Date": "2008-12-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 72.7699966430664
      },
      {
        "Date": "2008-12-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 71.52999877929688
      },
      {
        "Date": "2008-12-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 69.70999908447266
      },
      {
        "Date": "2008-12-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 67.73999786376953
      },
      {
        "Date": "2008-12-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 66.45999908447266
      },
      {"Date": "2008-12-16T00:00:00", "Bank": "GS", "Stock Price": 76},
      {
        "Date": "2008-12-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 78.77999877929688
      },
      {
        "Date": "2008-12-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 80.05000305175781
      },
      {
        "Date": "2008-12-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 80.7300033569336
      },
      {"Date": "2008-12-22T00:00:00", "Bank": "GS", "Stock Price": 77},
      {
        "Date": "2008-12-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 75.19999694824219
      },
      {
        "Date": "2008-12-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 76.44000244140625
      },
      {
        "Date": "2008-12-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 75.97000122070312
      },
      {
        "Date": "2008-12-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 76.55999755859375
      },
      {
        "Date": "2008-12-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 82.05999755859375
      },
      {
        "Date": "2008-12-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 84.38999938964844
      },
      {
        "Date": "2009-01-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 86.76000213623047
      },
      {
        "Date": "2009-01-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 88.77999877929688
      },
      {
        "Date": "2009-01-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 88.70999908447266
      },
      {"Date": "2009-01-07T00:00:00", "Bank": "GS", "Stock Price": 84.5},
      {
        "Date": "2009-01-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 85.41000366210938
      },
      {
        "Date": "2009-01-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 83.91999816894531
      },
      {
        "Date": "2009-01-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 77.66999816894531
      },
      {
        "Date": "2009-01-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 77.91999816894531
      },
      {
        "Date": "2009-01-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 75.69000244140625
      },
      {
        "Date": "2009-01-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 73.83000183105469
      },
      {
        "Date": "2009-01-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 73.05000305175781
      },
      {
        "Date": "2009-01-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 59.20000076293945
      },
      {
        "Date": "2009-01-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 69.9000015258789
      },
      {
        "Date": "2009-01-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 71.02999877929688
      },
      {
        "Date": "2009-01-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 74.91000366210938
      },
      {
        "Date": "2009-01-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 74.19999694824219
      },
      {
        "Date": "2009-01-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 78.26000213623047
      },
      {
        "Date": "2009-01-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 87.69999694824219
      },
      {
        "Date": "2009-01-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 82.72000122070312
      },
      {
        "Date": "2009-01-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 80.7300033569336
      },
      {
        "Date": "2009-02-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 83.56999969482422
      },
      {
        "Date": "2009-02-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 82.80999755859375
      },
      {
        "Date": "2009-02-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 87.97000122070312
      },
      {
        "Date": "2009-02-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 92.8499984741211
      },
      {
        "Date": "2009-02-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 96.56999969482422
      },
      {
        "Date": "2009-02-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 97.88999938964844
      },
      {
        "Date": "2009-02-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 90.4000015258789
      },
      {
        "Date": "2009-02-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 94.70999908447266
      },
      {
        "Date": "2009-02-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 95.58000183105469
      },
      {
        "Date": "2009-02-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 96.44999694824219
      },
      {
        "Date": "2009-02-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 85.70999908447266
      },
      {"Date": "2009-02-18T00:00:00", "Bank": "GS", "Stock Price": 84.5},
      {
        "Date": "2009-02-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 86.01000213623047
      },
      {
        "Date": "2009-02-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 84.58999633789062
      },
      {
        "Date": "2009-02-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 80.06999969482422
      },
      {
        "Date": "2009-02-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 92.9800033569336
      },
      {
        "Date": "2009-02-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 89.91999816894531
      },
      {
        "Date": "2009-02-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 92.1500015258789
      },
      {
        "Date": "2009-02-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 91.08000183105469
      },
      {
        "Date": "2009-03-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 86.2699966430664
      },
      {
        "Date": "2009-03-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 82.37000274658203
      },
      {
        "Date": "2009-03-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 85.47000122070312
      },
      {
        "Date": "2009-03-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 81.72000122070312
      },
      {
        "Date": "2009-03-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 75.6500015258789
      },
      {
        "Date": "2009-03-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 73.94999694824219
      },
      {
        "Date": "2009-03-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 85.27999877929688
      },
      {
        "Date": "2009-03-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 92.38999938964844
      },
      {"Date": "2009-03-12T00:00:00", "Bank": "GS", "Stock Price": 97.25},
      {
        "Date": "2009-03-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 98.80000305175781
      },
      {
        "Date": "2009-03-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 93.9000015258789
      },
      {
        "Date": "2009-03-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 98.98999786376953
      },
      {"Date": "2009-03-18T00:00:00", "Bank": "GS", "Stock Price": 105.25},
      {
        "Date": "2009-03-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 99.30000305175781
      },
      {
        "Date": "2009-03-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 97.31999969482422
      },
      {
        "Date": "2009-03-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 111.93000030517578
      },
      {
        "Date": "2009-03-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 110.5999984741211
      },
      {
        "Date": "2009-03-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 112.94999694824219
      },
      {
        "Date": "2009-03-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 111.98999786376953
      },
      {
        "Date": "2009-03-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 108.08000183105469
      },
      {
        "Date": "2009-03-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 100.45999908447266
      },
      {
        "Date": "2009-03-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 106.0199966430664
      },
      {
        "Date": "2009-04-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 110.29000091552734
      },
      {
        "Date": "2009-04-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 114.22000122070312
      },
      {
        "Date": "2009-04-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 119.4000015258789
      },
      {
        "Date": "2009-04-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 116.6500015258789
      },
      {
        "Date": "2009-04-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 116.08000183105469
      },
      {"Date": "2009-04-08T00:00:00", "Bank": "GS", "Stock Price": 114.75},
      {
        "Date": "2009-04-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 124.33000183105469
      },
      {
        "Date": "2009-04-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 130.14999389648438
      },
      {
        "Date": "2009-04-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 115.11000061035156
      },
      {
        "Date": "2009-04-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 121.19000244140625
      },
      {
        "Date": "2009-04-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 121.19000244140625
      },
      {
        "Date": "2009-04-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 120.5999984741211
      },
      {
        "Date": "2009-04-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 115.01000213623047
      },
      {
        "Date": "2009-04-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 120.36000061035156
      },
      {
        "Date": "2009-04-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 120.48999786376953
      },
      {
        "Date": "2009-04-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 122.80999755859375
      },
      {
        "Date": "2009-04-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 121.30000305175781
      },
      {
        "Date": "2009-04-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 120.9000015258789
      },
      {
        "Date": "2009-04-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 120.66999816894531
      },
      {
        "Date": "2009-04-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 127.18000030517578
      },
      {"Date": "2009-04-30T00:00:00", "Bank": "GS", "Stock Price": 128.5},
      {
        "Date": "2009-05-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 127.08000183105469
      },
      {
        "Date": "2009-05-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 134.16000366210938
      },
      {
        "Date": "2009-05-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 135.1999969482422
      },
      {
        "Date": "2009-05-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 139.22000122070312
      },
      {
        "Date": "2009-05-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 133.72999572753906
      },
      {
        "Date": "2009-05-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 139.58999633789062
      },
      {
        "Date": "2009-05-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 135.77999877929688
      },
      {
        "Date": "2009-05-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 135.41000366210938
      },
      {
        "Date": "2009-05-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 129.25999450683594
      },
      {
        "Date": "2009-05-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 133.60000610351562
      },
      {
        "Date": "2009-05-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 134.39999389648438
      },
      {
        "Date": "2009-05-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.14999389648438
      },
      {
        "Date": "2009-05-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 141.14999389648438
      },
      {
        "Date": "2009-05-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.44000244140625
      },
      {
        "Date": "2009-05-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.16000366210938
      },
      {
        "Date": "2009-05-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.35000610351562
      },
      {
        "Date": "2009-05-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.0500030517578
      },
      {
        "Date": "2009-05-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 140.00999450683594
      },
      {
        "Date": "2009-05-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.64999389648438
      },
      {
        "Date": "2009-05-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.57000732421875
      },
      {
        "Date": "2009-06-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.3300018310547
      },
      {
        "Date": "2009-06-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.1300048828125
      },
      {
        "Date": "2009-06-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.14999389648438
      },
      {
        "Date": "2009-06-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.47000122070312
      },
      {
        "Date": "2009-06-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.00999450683594
      },
      {
        "Date": "2009-06-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.35000610351562
      },
      {
        "Date": "2009-06-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.30999755859375
      },
      {
        "Date": "2009-06-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.67999267578125
      },
      {
        "Date": "2009-06-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 145.14999389648438
      },
      {
        "Date": "2009-06-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 145.63999938964844
      },
      {
        "Date": "2009-06-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.00999450683594
      },
      {
        "Date": "2009-06-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.16000366210938
      },
      {
        "Date": "2009-06-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 139.72999572753906
      },
      {
        "Date": "2009-06-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.08999633789062
      },
      {
        "Date": "2009-06-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.1300048828125
      },
      {
        "Date": "2009-06-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.00999450683594
      },
      {
        "Date": "2009-06-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 141.19000244140625
      },
      {
        "Date": "2009-06-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.64999389648438
      },
      {
        "Date": "2009-06-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.42999267578125
      },
      {
        "Date": "2009-06-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.74000549316406
      },
      {
        "Date": "2009-06-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.36000061035156
      },
      {
        "Date": "2009-06-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.44000244140625
      },
      {
        "Date": "2009-07-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.32000732421875
      },
      {
        "Date": "2009-07-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.49000549316406
      },
      {
        "Date": "2009-07-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.4600067138672
      },
      {
        "Date": "2009-07-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.5399932861328
      },
      {
        "Date": "2009-07-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 138.5500030517578
      },
      {
        "Date": "2009-07-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.2100067138672
      },
      {
        "Date": "2009-07-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 141.8699951171875
      },
      {
        "Date": "2009-07-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.44000244140625
      },
      {
        "Date": "2009-07-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.66000366210938
      },
      {
        "Date": "2009-07-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.25999450683594
      },
      {
        "Date": "2009-07-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.83999633789062
      },
      {
        "Date": "2009-07-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.83999633789062
      },
      {
        "Date": "2009-07-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.02999877929688
      },
      {
        "Date": "2009-07-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.8000030517578
      },
      {
        "Date": "2009-07-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.4600067138672
      },
      {
        "Date": "2009-07-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.4499969482422
      },
      {
        "Date": "2009-07-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.72000122070312
      },
      {
        "Date": "2009-07-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.8699951171875
      },
      {
        "Date": "2009-07-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.5399932861328
      },
      {
        "Date": "2009-07-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.44000244140625
      },
      {
        "Date": "2009-07-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.4199981689453
      },
      {
        "Date": "2009-07-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.3000030517578
      },
      {
        "Date": "2009-08-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.10000610351562
      },
      {
        "Date": "2009-08-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.1699981689453
      },
      {
        "Date": "2009-08-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.63999938964844
      },
      {"Date": "2009-08-06T00:00:00", "Bank": "GS", "Stock Price": 166.75},
      {
        "Date": "2009-08-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.64999389648438
      },
      {
        "Date": "2009-08-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.36000061035156
      },
      {
        "Date": "2009-08-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.22000122070312
      },
      {
        "Date": "2009-08-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.75999450683594
      },
      {
        "Date": "2009-08-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.47999572753906
      },
      {
        "Date": "2009-08-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.72999572753906
      },
      {"Date": "2009-08-17T00:00:00", "Bank": "GS", "Stock Price": 157.25},
      {
        "Date": "2009-08-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.47999572753906
      },
      {
        "Date": "2009-08-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.92999267578125
      },
      {
        "Date": "2009-08-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.3300018310547
      },
      {
        "Date": "2009-08-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.50999450683594
      },
      {
        "Date": "2009-08-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.5800018310547
      },
      {
        "Date": "2009-08-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.94000244140625
      },
      {
        "Date": "2009-08-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.9499969482422
      },
      {
        "Date": "2009-08-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.02000427246094
      },
      {
        "Date": "2009-08-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.4199981689453
      },
      {
        "Date": "2009-08-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.4600067138672
      },
      {
        "Date": "2009-09-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.1699981689453
      },
      {
        "Date": "2009-09-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.5399932861328
      },
      {
        "Date": "2009-09-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.66000366210938
      },
      {
        "Date": "2009-09-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.97000122070312
      },
      {
        "Date": "2009-09-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.22000122070312
      },
      {
        "Date": "2009-09-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.27000427246094
      },
      {
        "Date": "2009-09-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.8699951171875
      },
      {
        "Date": "2009-09-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.6999969482422
      },
      {
        "Date": "2009-09-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.7100067138672
      },
      {
        "Date": "2009-09-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.66000366210938
      },
      {
        "Date": "2009-09-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.8699951171875
      },
      {
        "Date": "2009-09-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 181.4600067138672
      },
      {
        "Date": "2009-09-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.17999267578125
      },
      {
        "Date": "2009-09-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 182.38999938964844
      },
      {
        "Date": "2009-09-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 185.52000427246094
      },
      {
        "Date": "2009-09-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.63999938964844
      },
      {
        "Date": "2009-09-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.05999755859375
      },
      {"Date": "2009-09-25T00:00:00", "Bank": "GS", "Stock Price": 179.5},
      {"Date": "2009-09-28T00:00:00", "Bank": "GS", "Stock Price": 182.5},
      {
        "Date": "2009-09-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.5800018310547
      },
      {
        "Date": "2009-09-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 184.35000610351562
      },
      {
        "Date": "2009-10-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.99000549316406
      },
      {
        "Date": "2009-10-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.61000061035156
      },
      {
        "Date": "2009-10-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 186.47000122070312
      },
      {
        "Date": "2009-10-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 186.97999572753906
      },
      {
        "Date": "2009-10-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.47999572753906
      },
      {
        "Date": "2009-10-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.1699981689453
      },
      {
        "Date": "2009-10-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 189.3000030517578
      },
      {
        "Date": "2009-10-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 190.14999389648438
      },
      {
        "Date": "2009-10-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 187.22999572753906
      },
      {
        "Date": "2009-10-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 192.27999877929688
      },
      {
        "Date": "2009-10-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 188.6300048828125
      },
      {
        "Date": "2009-10-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 184.3699951171875
      },
      {"Date": "2009-10-19T00:00:00", "Bank": "GS", "Stock Price": 185.5},
      {
        "Date": "2009-10-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 184.9600067138672
      },
      {
        "Date": "2009-10-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.25999450683594
      },
      {
        "Date": "2009-10-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 183.69000244140625
      },
      {
        "Date": "2009-10-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 180.36000061035156
      },
      {
        "Date": "2009-10-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.3699951171875
      },
      {
        "Date": "2009-10-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.61000061035156
      },
      {
        "Date": "2009-10-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.16000366210938
      },
      {
        "Date": "2009-10-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.5800018310547
      },
      {
        "Date": "2009-10-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.1699981689453
      },
      {
        "Date": "2009-11-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.67999267578125
      },
      {
        "Date": "2009-11-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.61000061035156
      },
      {"Date": "2009-11-04T00:00:00", "Bank": "GS", "Stock Price": 169.5},
      {
        "Date": "2009-11-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.39999389648438
      },
      {
        "Date": "2009-11-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.77999877929688
      },
      {
        "Date": "2009-11-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.57000732421875
      },
      {
        "Date": "2009-11-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.50999450683594
      },
      {
        "Date": "2009-11-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.85000610351562
      },
      {
        "Date": "2009-11-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 178.47999572753906
      },
      {
        "Date": "2009-11-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.75999450683594
      },
      {"Date": "2009-11-16T00:00:00", "Bank": "GS", "Stock Price": 177.25},
      {
        "Date": "2009-11-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.60000610351562
      },
      {
        "Date": "2009-11-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.89999389648438
      },
      {
        "Date": "2009-11-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.8300018310547
      },
      {
        "Date": "2009-11-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.00999450683594
      },
      {"Date": "2009-11-23T00:00:00", "Bank": "GS", "Stock Price": 172},
      {
        "Date": "2009-11-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.1300048828125
      },
      {
        "Date": "2009-11-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.9199981689453
      },
      {
        "Date": "2009-11-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.16000366210938
      },
      {
        "Date": "2009-11-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.66000366210938
      },
      {
        "Date": "2009-12-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.6300048828125
      },
      {
        "Date": "2009-12-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.66000366210938
      },
      {
        "Date": "2009-12-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.3000030517578
      },
      {
        "Date": "2009-12-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.24000549316406
      },
      {
        "Date": "2009-12-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.85000610351562
      },
      {
        "Date": "2009-12-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.83999633789062
      },
      {
        "Date": "2009-12-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.44000244140625
      },
      {
        "Date": "2009-12-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.72999572753906
      },
      {"Date": "2009-12-11T00:00:00", "Bank": "GS", "Stock Price": 166},
      {
        "Date": "2009-12-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.10000610351562
      },
      {
        "Date": "2009-12-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.74000549316406
      },
      {
        "Date": "2009-12-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.99000549316406
      },
      {
        "Date": "2009-12-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.92999267578125
      },
      {
        "Date": "2009-12-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.19000244140625
      },
      {
        "Date": "2009-12-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.4499969482422
      },
      {
        "Date": "2009-12-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.60000610351562
      },
      {
        "Date": "2009-12-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.6300048828125
      },
      {
        "Date": "2009-12-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.97000122070312
      },
      {
        "Date": "2009-12-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.75999450683594
      },
      {
        "Date": "2009-12-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.1199951171875
      },
      {
        "Date": "2009-12-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.6999969482422
      },
      {
        "Date": "2009-12-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.83999633789062
      },
      {
        "Date": "2010-01-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.0800018310547
      },
      {
        "Date": "2010-01-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.13999938964844
      },
      {
        "Date": "2010-01-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.25999450683594
      },
      {
        "Date": "2010-01-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.6699981689453
      },
      {
        "Date": "2010-01-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.30999755859375
      },
      {
        "Date": "2010-01-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.55999755859375
      },
      {
        "Date": "2010-01-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.82000732421875
      },
      {
        "Date": "2010-01-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.07000732421875
      },
      {
        "Date": "2010-01-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.52999877929688
      },
      {
        "Date": "2010-01-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.2100067138672
      },
      {
        "Date": "2010-01-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.86000061035156
      },
      {
        "Date": "2010-01-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.7899932861328
      },
      {
        "Date": "2010-01-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.8699951171875
      },
      {
        "Date": "2010-01-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 154.1199951171875
      },
      {
        "Date": "2010-01-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 154.97999572753906
      },
      {
        "Date": "2010-01-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 150.8800048828125
      },
      {"Date": "2010-01-27T00:00:00", "Bank": "GS", "Stock Price": 151.5},
      {
        "Date": "2010-01-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.2899932861328
      },
      {
        "Date": "2010-01-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.72000122070312
      },
      {
        "Date": "2010-02-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.1300048828125
      },
      {
        "Date": "2010-02-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.94000244140625
      },
      {
        "Date": "2010-02-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.22999572753906
      },
      {
        "Date": "2010-02-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 150.67999267578125
      },
      {
        "Date": "2010-02-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 154.16000366210938
      },
      {
        "Date": "2010-02-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 151.10000610351562
      },
      {
        "Date": "2010-02-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.49000549316406
      },
      {
        "Date": "2010-02-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.6300048828125
      },
      {
        "Date": "2010-02-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 154.0500030517578
      },
      {
        "Date": "2010-02-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.92999267578125
      },
      {
        "Date": "2010-02-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.39999389648438
      },
      {
        "Date": "2010-02-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.25999450683594
      },
      {
        "Date": "2010-02-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.72999572753906
      },
      {
        "Date": "2010-02-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.17999267578125
      },
      {
        "Date": "2010-02-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.7100067138672
      },
      {
        "Date": "2010-02-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.6999969482422
      },
      {
        "Date": "2010-02-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.3300018310547
      },
      {
        "Date": "2010-02-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.44000244140625
      },
      {
        "Date": "2010-02-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.35000610351562
      },
      {
        "Date": "2010-03-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.5399932861328
      },
      {"Date": "2010-03-02T00:00:00", "Bank": "GS", "Stock Price": 158.75},
      {
        "Date": "2010-03-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.72000122070312
      },
      {
        "Date": "2010-03-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.61000061035156
      },
      {
        "Date": "2010-03-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.17999267578125
      },
      {
        "Date": "2010-03-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.83999633789062
      },
      {
        "Date": "2010-03-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.85000610351562
      },
      {
        "Date": "2010-03-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.94000244140625
      },
      {
        "Date": "2010-03-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.50999450683594
      },
      {
        "Date": "2010-03-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.9600067138672
      },
      {
        "Date": "2010-03-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.52999877929688
      },
      {
        "Date": "2010-03-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.19000244140625
      },
      {
        "Date": "2010-03-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.63999938964844
      },
      {
        "Date": "2010-03-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.4499969482422
      },
      {
        "Date": "2010-03-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.89999389648438
      },
      {
        "Date": "2010-03-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.16000366210938
      },
      {
        "Date": "2010-03-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.8300018310547
      },
      {
        "Date": "2010-03-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.41000366210938
      },
      {
        "Date": "2010-03-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.89999389648438
      },
      {
        "Date": "2010-03-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.8699951171875
      },
      {
        "Date": "2010-03-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 174.0500030517578
      },
      {
        "Date": "2010-03-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.3800048828125
      },
      {
        "Date": "2010-03-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.6300048828125
      },
      {
        "Date": "2010-04-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 170.22000122070312
      },
      {
        "Date": "2010-04-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 173.16000366210938
      },
      {
        "Date": "2010-04-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 172.89999389648438
      },
      {
        "Date": "2010-04-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 176.36000061035156
      },
      {"Date": "2010-04-08T00:00:00", "Bank": "GS", "Stock Price": 179.5},
      {
        "Date": "2010-04-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 179.1199951171875
      },
      {
        "Date": "2010-04-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 177.83999633789062
      },
      {"Date": "2010-04-13T00:00:00", "Bank": "GS", "Stock Price": 179.25},
      {
        "Date": "2010-04-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 184.9199981689453
      },
      {
        "Date": "2010-04-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 184.27000427246094
      },
      {
        "Date": "2010-04-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.6999969482422
      },
      {
        "Date": "2010-04-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.32000732421875
      },
      {
        "Date": "2010-04-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.97999572753906
      },
      {
        "Date": "2010-04-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.92999267578125
      },
      {
        "Date": "2010-04-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.0500030517578
      },
      {
        "Date": "2010-04-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.39999389648438
      },
      {
        "Date": "2010-04-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.02999877929688
      },
      {
        "Date": "2010-04-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.0399932861328
      },
      {
        "Date": "2010-04-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.00999450683594
      },
      {
        "Date": "2010-04-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.24000549316406
      },
      {
        "Date": "2010-04-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 145.1999969482422
      },
      {"Date": "2010-05-03T00:00:00", "Bank": "GS", "Stock Price": 149.5},
      {
        "Date": "2010-05-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.4499969482422
      },
      {
        "Date": "2010-05-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.19000244140625
      },
      {
        "Date": "2010-05-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.32000732421875
      },
      {
        "Date": "2010-05-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.99000549316406
      },
      {
        "Date": "2010-05-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.8300018310547
      },
      {
        "Date": "2010-05-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 141.97000122070312
      },
      {
        "Date": "2010-05-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.1999969482422
      },
      {
        "Date": "2010-05-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.64999389648438
      },
      {
        "Date": "2010-05-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.22999572753906
      },
      {
        "Date": "2010-05-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.63999938964844
      },
      {
        "Date": "2010-05-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.36000061035156
      },
      {
        "Date": "2010-05-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 140.10000610351562
      },
      {
        "Date": "2010-05-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.10000610351562
      },
      {
        "Date": "2010-05-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 140.6199951171875
      },
      {
        "Date": "2010-05-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.69000244140625
      },
      {
        "Date": "2010-05-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 142.55999755859375
      },
      {
        "Date": "2010-05-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 140.3000030517578
      },
      {
        "Date": "2010-05-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.9499969482422
      },
      {
        "Date": "2010-05-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.25999450683594
      },
      {
        "Date": "2010-06-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 141.86000061035156
      },
      {
        "Date": "2010-06-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.8300018310547
      },
      {
        "Date": "2010-06-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.0399932861328
      },
      {"Date": "2010-06-04T00:00:00", "Bank": "GS", "Stock Price": 142.25},
      {
        "Date": "2010-06-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 138.67999267578125
      },
      {
        "Date": "2010-06-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.77999877929688
      },
      {
        "Date": "2010-06-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.8000030517578
      },
      {
        "Date": "2010-06-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 133.77000427246094
      },
      {
        "Date": "2010-06-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 135.63999938964844
      },
      {
        "Date": "2010-06-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 133.44000244140625
      },
      {
        "Date": "2010-06-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.89999389648438
      },
      {
        "Date": "2010-06-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.05999755859375
      },
      {
        "Date": "2010-06-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.32000732421875
      },
      {
        "Date": "2010-06-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 138.17999267578125
      },
      {
        "Date": "2010-06-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 137.74000549316406
      },
      {
        "Date": "2010-06-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 134.7899932861328
      },
      {
        "Date": "2010-06-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 135.07000732421875
      },
      {
        "Date": "2010-06-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 134.97999572753906
      },
      {
        "Date": "2010-06-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 139.66000366210938
      },
      {
        "Date": "2010-06-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.66000366210938
      },
      {
        "Date": "2010-06-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 133.75999450683594
      },
      {
        "Date": "2010-06-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 131.27000427246094
      },
      {
        "Date": "2010-07-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 131.13999938964844
      },
      {
        "Date": "2010-07-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 131.0800018310547
      },
      {
        "Date": "2010-07-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 132.25999450683594
      },
      {
        "Date": "2010-07-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 135.8300018310547
      },
      {
        "Date": "2010-07-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 135.4600067138672
      },
      {
        "Date": "2010-07-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 138.05999755859375
      },
      {"Date": "2010-07-12T00:00:00", "Bank": "GS", "Stock Price": 137.25},
      {"Date": "2010-07-13T00:00:00", "Bank": "GS", "Stock Price": 140.25},
      {
        "Date": "2010-07-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 139.05999755859375
      },
      {
        "Date": "2010-07-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 145.22000122070312
      },
      {
        "Date": "2010-07-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.1699981689453
      },
      {
        "Date": "2010-07-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 145.67999267578125
      },
      {
        "Date": "2010-07-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.91000366210938
      },
      {
        "Date": "2010-07-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.99000549316406
      },
      {
        "Date": "2010-07-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.5500030517578
      },
      {
        "Date": "2010-07-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.3800048828125
      },
      {
        "Date": "2010-07-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.1999969482422
      },
      {
        "Date": "2010-07-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.22999572753906
      },
      {
        "Date": "2010-07-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.1999969482422
      },
      {
        "Date": "2010-07-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.5800018310547
      },
      {
        "Date": "2010-07-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 150.82000732421875
      },
      {
        "Date": "2010-08-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.74000549316406
      },
      {
        "Date": "2010-08-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.19000244140625
      },
      {
        "Date": "2010-08-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.41000366210938
      },
      {
        "Date": "2010-08-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.9199981689453
      },
      {
        "Date": "2010-08-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.17999267578125
      },
      {
        "Date": "2010-08-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.39999389648438
      },
      {
        "Date": "2010-08-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.89999389648438
      },
      {"Date": "2010-08-11T00:00:00", "Bank": "GS", "Stock Price": 149.25},
      {
        "Date": "2010-08-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.4199981689453
      },
      {
        "Date": "2010-08-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.0800018310547
      },
      {
        "Date": "2010-08-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.75999450683594
      },
      {
        "Date": "2010-08-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.58999633789062
      },
      {
        "Date": "2010-08-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.1999969482422
      },
      {
        "Date": "2010-08-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.0500030517578
      },
      {
        "Date": "2010-08-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.24000549316406
      },
      {
        "Date": "2010-08-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.74000549316406
      },
      {
        "Date": "2010-08-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 143.9499969482422
      },
      {
        "Date": "2010-08-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.67999267578125
      },
      {
        "Date": "2010-08-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 141.80999755859375
      },
      {"Date": "2010-08-27T00:00:00", "Bank": "GS", "Stock Price": 139.75},
      {
        "Date": "2010-08-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.66000366210938
      },
      {
        "Date": "2010-08-31T00:00:00",
        "Bank": "GS",
        "Stock Price": 136.92999267578125
      },
      {
        "Date": "2010-09-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 139.74000549316406
      },
      {
        "Date": "2010-09-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 139.77999877929688
      },
      {
        "Date": "2010-09-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.2899932861328
      },
      {
        "Date": "2010-09-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 145.2100067138672
      },
      {
        "Date": "2010-09-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.5399932861328
      },
      {
        "Date": "2010-09-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.13999938964844
      },
      {
        "Date": "2010-09-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 150.38999938964844
      },
      {
        "Date": "2010-09-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 154.3699951171875
      },
      {
        "Date": "2010-09-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.52999877929688
      },
      {
        "Date": "2010-09-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.55999755859375
      },
      {
        "Date": "2010-09-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.22999572753906
      },
      {
        "Date": "2010-09-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 150.97999572753906
      },
      {
        "Date": "2010-09-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 151.89999389648438
      },
      {
        "Date": "2010-09-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 151.39999389648438
      },
      {
        "Date": "2010-09-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 148.07000732421875
      },
      {
        "Date": "2010-09-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.91000366210938
      },
      {
        "Date": "2010-09-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.27999877929688
      },
      {"Date": "2010-09-27T00:00:00", "Bank": "GS", "Stock Price": 146},
      {
        "Date": "2010-09-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 145.00999450683594
      },
      {
        "Date": "2010-09-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.4199981689453
      },
      {
        "Date": "2010-09-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 144.5800018310547
      },
      {
        "Date": "2010-10-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 147.6999969482422
      },
      {
        "Date": "2010-10-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 146.57000732421875
      },
      {
        "Date": "2010-10-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 149.57000732421875
      },
      {
        "Date": "2010-10-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 150.83999633789062
      },
      {
        "Date": "2010-10-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 151.11000061035156
      },
      {
        "Date": "2010-10-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.66000366210938
      },
      {
        "Date": "2010-10-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 152.1999969482422
      },
      {
        "Date": "2010-10-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 155.2100067138672
      },
      {
        "Date": "2010-10-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 154.72999572753906
      },
      {
        "Date": "2010-10-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 151.58999633789062
      },
      {
        "Date": "2010-10-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 150.69000244140625
      },
      {
        "Date": "2010-10-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 153.6999969482422
      },
      {
        "Date": "2010-10-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.72000122070312
      },
      {
        "Date": "2010-10-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.60000610351562
      },
      {
        "Date": "2010-10-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.3000030517578
      },
      {
        "Date": "2010-10-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.75999450683594
      },
      {
        "Date": "2010-10-25T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.38999938964844
      },
      {
        "Date": "2010-10-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.2899932861328
      },
      {
        "Date": "2010-10-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.14999389648438
      },
      {
        "Date": "2010-10-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 163.24000549316406
      },
      {
        "Date": "2010-10-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.1300048828125
      },
      {
        "Date": "2010-11-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.57000732421875
      },
      {
        "Date": "2010-11-02T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.82000732421875
      },
      {
        "Date": "2010-11-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.6300048828125
      },
      {
        "Date": "2010-11-04T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.38999938964844
      },
      {
        "Date": "2010-11-05T00:00:00",
        "Bank": "GS",
        "Stock Price": 171.07000732421875
      },
      {
        "Date": "2010-11-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.1999969482422
      },
      {
        "Date": "2010-11-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.5500030517578
      },
      {
        "Date": "2010-11-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.22000122070312
      },
      {
        "Date": "2010-11-11T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.7100067138672
      },
      {
        "Date": "2010-11-12T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.8300018310547
      },
      {
        "Date": "2010-11-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.22000122070312
      },
      {
        "Date": "2010-11-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.10000610351562
      },
      {
        "Date": "2010-11-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.88999938964844
      },
      {
        "Date": "2010-11-18T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.35000610351562
      },
      {
        "Date": "2010-11-19T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.6699981689453
      },
      {
        "Date": "2010-11-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.0500030517578
      },
      {
        "Date": "2010-11-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 157.77999877929688
      },
      {
        "Date": "2010-11-24T00:00:00",
        "Bank": "GS",
        "Stock Price": 160.25999450683594
      },
      {
        "Date": "2010-11-26T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.22000122070312
      },
      {
        "Date": "2010-11-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 159.27999877929688
      },
      {
        "Date": "2010-11-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 156.13999938964844
      },
      {
        "Date": "2010-12-01T00:00:00",
        "Bank": "GS",
        "Stock Price": 158.4499969482422
      },
      {"Date": "2010-12-02T00:00:00", "Bank": "GS", "Stock Price": 162.5},
      {
        "Date": "2010-12-03T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.30999755859375
      },
      {
        "Date": "2010-12-06T00:00:00",
        "Bank": "GS",
        "Stock Price": 162.64999389648438
      },
      {
        "Date": "2010-12-07T00:00:00",
        "Bank": "GS",
        "Stock Price": 161.58999633789062
      },
      {
        "Date": "2010-12-08T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.13999938964844
      },
      {
        "Date": "2010-12-09T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.4499969482422
      },
      {
        "Date": "2010-12-10T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.47000122070312
      },
      {
        "Date": "2010-12-13T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.47999572753906
      },
      {
        "Date": "2010-12-14T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.3300018310547
      },
      {
        "Date": "2010-12-15T00:00:00",
        "Bank": "GS",
        "Stock Price": 165.2100067138672
      },
      {
        "Date": "2010-12-16T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.4600067138672
      },
      {
        "Date": "2010-12-17T00:00:00",
        "Bank": "GS",
        "Stock Price": 164.0399932861328
      },
      {
        "Date": "2010-12-20T00:00:00",
        "Bank": "GS",
        "Stock Price": 166.0500030517578
      },
      {
        "Date": "2010-12-21T00:00:00",
        "Bank": "GS",
        "Stock Price": 168.22999572753906
      },
      {
        "Date": "2010-12-22T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.60000610351562
      },
      {
        "Date": "2010-12-23T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.60000610351562
      },
      {
        "Date": "2010-12-27T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.8300018310547
      },
      {
        "Date": "2010-12-28T00:00:00",
        "Bank": "GS",
        "Stock Price": 169.19000244140625
      },
      {
        "Date": "2010-12-29T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.6300048828125
      },
      {
        "Date": "2010-12-30T00:00:00",
        "Bank": "GS",
        "Stock Price": 167.63999938964844
      },
      {
        "Date": "2007-01-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.06999969482422
      },
      {
        "Date": "2007-01-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.189998626708984
      },
      {
        "Date": "2007-01-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.790000915527344
      },
      {
        "Date": "2007-01-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.95000076293945
      },
      {"Date": "2007-01-09T00:00:00", "Bank": "JPM", "Stock Price": 47.75},
      {
        "Date": "2007-01-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.099998474121094
      },
      {
        "Date": "2007-01-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.310001373291016
      },
      {
        "Date": "2007-01-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.9900016784668
      },
      {
        "Date": "2007-01-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.38999938964844
      },
      {
        "Date": "2007-01-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.43000030517578
      },
      {
        "Date": "2007-01-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.150001525878906
      },
      {
        "Date": "2007-01-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.7599983215332
      },
      {
        "Date": "2007-01-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.65999984741211
      },
      {
        "Date": "2007-01-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.83000183105469
      },
      {
        "Date": "2007-01-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.36000061035156
      },
      {
        "Date": "2007-01-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.209999084472656
      },
      {
        "Date": "2007-01-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.70000076293945
      },
      {
        "Date": "2007-01-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.470001220703125
      },
      {
        "Date": "2007-01-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.18000030517578
      },
      {
        "Date": "2007-01-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.93000030517578
      },
      {
        "Date": "2007-02-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.209999084472656
      },
      {
        "Date": "2007-02-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.93000030517578
      },
      {
        "Date": "2007-02-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.959999084472656
      },
      {"Date": "2007-02-06T00:00:00", "Bank": "JPM", "Stock Price": 51},
      {
        "Date": "2007-02-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.209999084472656
      },
      {
        "Date": "2007-02-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.93000030517578
      },
      {
        "Date": "2007-02-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.41999816894531
      },
      {
        "Date": "2007-02-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.439998626708984
      },
      {
        "Date": "2007-02-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.95000076293945
      },
      {
        "Date": "2007-02-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.41999816894531
      },
      {
        "Date": "2007-02-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.209999084472656
      },
      {"Date": "2007-02-16T00:00:00", "Bank": "JPM", "Stock Price": 51.25},
      {
        "Date": "2007-02-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.630001068115234
      },
      {
        "Date": "2007-02-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.650001525878906
      },
      {
        "Date": "2007-02-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.63999938964844
      },
      {
        "Date": "2007-02-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.029998779296875
      },
      {
        "Date": "2007-02-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.810001373291016
      },
      {
        "Date": "2007-02-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.220001220703125
      },
      {
        "Date": "2007-02-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.38999938964844
      },
      {
        "Date": "2007-03-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.20000076293945
      },
      {
        "Date": "2007-03-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.189998626708984
      },
      {
        "Date": "2007-03-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.540000915527344
      },
      {
        "Date": "2007-03-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.52000045776367
      },
      {
        "Date": "2007-03-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.36000061035156
      },
      {
        "Date": "2007-03-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.7400016784668
      },
      {
        "Date": "2007-03-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.81999969482422
      },
      {
        "Date": "2007-03-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.84000015258789
      },
      {
        "Date": "2007-03-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.70000076293945
      },
      {
        "Date": "2007-03-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.29999923706055
      },
      {
        "Date": "2007-03-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.70000076293945
      },
      {
        "Date": "2007-03-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.029998779296875
      },
      {
        "Date": "2007-03-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.58000183105469
      },
      {"Date": "2007-03-20T00:00:00", "Bank": "JPM", "Stock Price": 47.75},
      {
        "Date": "2007-03-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.04999923706055
      },
      {
        "Date": "2007-03-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.470001220703125
      },
      {
        "Date": "2007-03-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.52000045776367
      },
      {
        "Date": "2007-03-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.70000076293945
      },
      {
        "Date": "2007-03-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.56999969482422
      },
      {
        "Date": "2007-03-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.9900016784668
      },
      {"Date": "2007-03-29T00:00:00", "Bank": "JPM", "Stock Price": 48.5},
      {
        "Date": "2007-03-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.380001068115234
      },
      {
        "Date": "2007-04-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.2400016784668
      },
      {
        "Date": "2007-04-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.560001373291016
      },
      {
        "Date": "2007-04-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.560001373291016
      },
      {
        "Date": "2007-04-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.77000045776367
      },
      {"Date": "2007-04-09T00:00:00", "Bank": "JPM", "Stock Price": 49},
      {
        "Date": "2007-04-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.2400016784668
      },
      {
        "Date": "2007-04-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.150001525878906
      },
      {
        "Date": "2007-04-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.20000076293945
      },
      {
        "Date": "2007-04-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.09000015258789
      },
      {
        "Date": "2007-04-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.970001220703125
      },
      {
        "Date": "2007-04-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.18000030517578
      },
      {
        "Date": "2007-04-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.06999969482422
      },
      {
        "Date": "2007-04-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.09000015258789
      },
      {
        "Date": "2007-04-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.540000915527344
      },
      {
        "Date": "2007-04-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.279998779296875
      },
      {
        "Date": "2007-04-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.15999984741211
      },
      {
        "Date": "2007-04-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.81999969482422
      },
      {
        "Date": "2007-04-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.939998626708984
      },
      {
        "Date": "2007-04-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.54999923706055
      },
      {
        "Date": "2007-04-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.099998474121094
      },
      {
        "Date": "2007-05-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.2599983215332
      },
      {
        "Date": "2007-05-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.54999923706055
      },
      {
        "Date": "2007-05-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.70000076293945
      },
      {
        "Date": "2007-05-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.630001068115234
      },
      {
        "Date": "2007-05-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.72999954223633
      },
      {
        "Date": "2007-05-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.45000076293945
      },
      {
        "Date": "2007-05-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 53.20000076293945
      },
      {"Date": "2007-05-10T00:00:00", "Bank": "JPM", "Stock Price": 52},
      {
        "Date": "2007-05-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.150001525878906
      },
      {
        "Date": "2007-05-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.83000183105469
      },
      {
        "Date": "2007-05-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.029998779296875
      },
      {
        "Date": "2007-05-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.97999954223633
      },
      {
        "Date": "2007-05-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.560001373291016
      },
      {
        "Date": "2007-05-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.540000915527344
      },
      {
        "Date": "2007-05-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.560001373291016
      },
      {
        "Date": "2007-05-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.290000915527344
      },
      {
        "Date": "2007-05-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.9900016784668
      },
      {
        "Date": "2007-05-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.59000015258789
      },
      {
        "Date": "2007-05-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.63999938964844
      },
      {
        "Date": "2007-05-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.81999969482422
      },
      {
        "Date": "2007-05-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 52.060001373291016
      },
      {
        "Date": "2007-05-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.83000183105469
      },
      {
        "Date": "2007-06-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.900001525878906
      },
      {
        "Date": "2007-06-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.56999969482422
      },
      {
        "Date": "2007-06-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 51.220001220703125
      },
      {
        "Date": "2007-06-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.560001373291016
      },
      {
        "Date": "2007-06-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.81999969482422
      },
      {
        "Date": "2007-06-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.40999984741211
      },
      {
        "Date": "2007-06-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.43000030517578
      },
      {
        "Date": "2007-06-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.349998474121094
      },
      {
        "Date": "2007-06-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.290000915527344
      },
      {
        "Date": "2007-06-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.31999969482422
      },
      {
        "Date": "2007-06-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.560001373291016
      },
      {
        "Date": "2007-06-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.43000030517578
      },
      {
        "Date": "2007-06-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.849998474121094
      },
      {
        "Date": "2007-06-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.459999084472656
      },
      {
        "Date": "2007-06-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.84000015258789
      },
      {
        "Date": "2007-06-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.720001220703125
      },
      {
        "Date": "2007-06-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.36000061035156
      },
      {
        "Date": "2007-06-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.599998474121094
      },
      {
        "Date": "2007-06-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.2400016784668
      },
      {
        "Date": "2007-06-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.959999084472656
      },
      {
        "Date": "2007-06-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.45000076293945
      },
      {
        "Date": "2007-07-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.150001525878906
      },
      {
        "Date": "2007-07-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.34000015258789
      },
      {
        "Date": "2007-07-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.790000915527344
      },
      {
        "Date": "2007-07-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.970001220703125
      },
      {
        "Date": "2007-07-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.790000915527344
      },
      {
        "Date": "2007-07-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.5099983215332
      },
      {
        "Date": "2007-07-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.130001068115234
      },
      {
        "Date": "2007-07-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.529998779296875
      },
      {
        "Date": "2007-07-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 50.04999923706055
      },
      {
        "Date": "2007-07-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.83000183105469
      },
      {
        "Date": "2007-07-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.91999816894531
      },
      {
        "Date": "2007-07-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.880001068115234
      },
      {
        "Date": "2007-07-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.619998931884766
      },
      {
        "Date": "2007-07-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.560001373291016
      },
      {
        "Date": "2007-07-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.150001525878906
      },
      {
        "Date": "2007-07-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.34000015258789
      },
      {
        "Date": "2007-07-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.27000045776367
      },
      {
        "Date": "2007-07-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.08000183105469
      },
      {
        "Date": "2007-07-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.22999954223633
      },
      {"Date": "2007-07-30T00:00:00", "Bank": "JPM", "Stock Price": 44.75},
      {
        "Date": "2007-07-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.0099983215332
      },
      {
        "Date": "2007-08-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.380001068115234
      },
      {
        "Date": "2007-08-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.59000015258789
      },
      {
        "Date": "2007-08-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.650001525878906
      },
      {
        "Date": "2007-08-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.11000061035156
      },
      {
        "Date": "2007-08-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.34000015258789
      },
      {
        "Date": "2007-08-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.5099983215332
      },
      {
        "Date": "2007-08-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.16999816894531
      },
      {"Date": "2007-08-10T00:00:00", "Bank": "JPM", "Stock Price": 44.25},
      {
        "Date": "2007-08-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.83000183105469
      },
      {
        "Date": "2007-08-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.29999923706055
      },
      {"Date": "2007-08-15T00:00:00", "Bank": "JPM", "Stock Price": 43},
      {
        "Date": "2007-08-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.470001220703125
      },
      {
        "Date": "2007-08-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.0099983215332
      },
      {
        "Date": "2007-08-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.4900016784668
      },
      {
        "Date": "2007-08-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.20000076293945
      },
      {"Date": "2007-08-22T00:00:00", "Bank": "JPM", "Stock Price": 46},
      {
        "Date": "2007-08-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.66999816894531
      },
      {
        "Date": "2007-08-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.95000076293945
      },
      {
        "Date": "2007-08-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.90999984741211
      },
      {
        "Date": "2007-08-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.599998474121094
      },
      {
        "Date": "2007-08-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.130001068115234
      },
      {
        "Date": "2007-08-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.970001220703125
      },
      {
        "Date": "2007-08-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.52000045776367
      },
      {
        "Date": "2007-09-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.29999923706055
      },
      {
        "Date": "2007-09-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.16999816894531
      },
      {
        "Date": "2007-09-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.209999084472656
      },
      {
        "Date": "2007-09-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.52000045776367
      },
      {
        "Date": "2007-09-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.93000030517578
      },
      {
        "Date": "2007-09-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.540000915527344
      },
      {
        "Date": "2007-09-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.470001220703125
      },
      {
        "Date": "2007-09-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.599998474121094
      },
      {
        "Date": "2007-09-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.540000915527344
      },
      {
        "Date": "2007-09-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.290000915527344
      },
      {
        "Date": "2007-09-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.81999969482422
      },
      {
        "Date": "2007-09-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.56999969482422
      },
      {
        "Date": "2007-09-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.959999084472656
      },
      {
        "Date": "2007-09-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.130001068115234
      },
      {
        "Date": "2007-09-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.34000015258789
      },
      {
        "Date": "2007-09-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.099998474121094
      },
      {
        "Date": "2007-09-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.130001068115234
      },
      {
        "Date": "2007-09-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.209999084472656
      },
      {
        "Date": "2007-09-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.81999969482422
      },
      {
        "Date": "2007-10-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.810001373291016
      },
      {
        "Date": "2007-10-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.15999984741211
      },
      {"Date": "2007-10-03T00:00:00", "Bank": "JPM", "Stock Price": 47},
      {"Date": "2007-10-04T00:00:00", "Bank": "JPM", "Stock Price": 47.25},
      {
        "Date": "2007-10-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.58000183105469
      },
      {
        "Date": "2007-10-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.439998626708984
      },
      {
        "Date": "2007-10-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.56999969482422
      },
      {
        "Date": "2007-10-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.90999984741211
      },
      {
        "Date": "2007-10-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.65999984741211
      },
      {
        "Date": "2007-10-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.81999969482422
      },
      {
        "Date": "2007-10-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.27000045776367
      },
      {
        "Date": "2007-10-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.11000061035156
      },
      {
        "Date": "2007-10-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.369998931884766
      },
      {
        "Date": "2007-10-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.900001525878906
      },
      {
        "Date": "2007-10-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.02000045776367
      },
      {
        "Date": "2007-10-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.369998931884766
      },
      {
        "Date": "2007-10-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.939998626708984
      },
      {
        "Date": "2007-10-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.27000045776367
      },
      {
        "Date": "2007-10-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.04999923706055
      },
      {
        "Date": "2007-10-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.31999969482422
      },
      {
        "Date": "2007-10-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.66999816894531
      },
      {
        "Date": "2007-10-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.560001373291016
      },
      {"Date": "2007-10-31T00:00:00", "Bank": "JPM", "Stock Price": 47},
      {
        "Date": "2007-11-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.31999969482422
      },
      {
        "Date": "2007-11-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.150001525878906
      },
      {
        "Date": "2007-11-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.77000045776367
      },
      {
        "Date": "2007-11-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.11000061035156
      },
      {
        "Date": "2007-11-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.2400016784668
      },
      {
        "Date": "2007-11-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.61000061035156
      },
      {
        "Date": "2007-11-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.310001373291016
      },
      {
        "Date": "2007-11-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.38999938964844
      },
      {
        "Date": "2007-11-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.04999923706055
      },
      {
        "Date": "2007-11-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.150001525878906
      },
      {
        "Date": "2007-11-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.529998779296875
      },
      {
        "Date": "2007-11-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.09000015258789
      },
      {
        "Date": "2007-11-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.369998931884766
      },
      {
        "Date": "2007-11-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.630001068115234
      },
      {
        "Date": "2007-11-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.68000030517578
      },
      {
        "Date": "2007-11-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.95000076293945
      },
      {
        "Date": "2007-11-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.459999084472656
      },
      {
        "Date": "2007-11-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.349998474121094
      },
      {
        "Date": "2007-11-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.959999084472656
      },
      {
        "Date": "2007-11-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.650001525878906
      },
      {
        "Date": "2007-11-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.619998931884766
      },
      {
        "Date": "2007-12-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.209999084472656
      },
      {
        "Date": "2007-12-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.150001525878906
      },
      {
        "Date": "2007-12-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.900001525878906
      },
      {
        "Date": "2007-12-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.209999084472656
      },
      {
        "Date": "2007-12-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.08000183105469
      },
      {
        "Date": "2007-12-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.41999816894531
      },
      {
        "Date": "2007-12-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.939998626708984
      },
      {
        "Date": "2007-12-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.150001525878906
      },
      {
        "Date": "2007-12-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.7599983215332
      },
      {
        "Date": "2007-12-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.20000076293945
      },
      {
        "Date": "2007-12-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.529998779296875
      },
      {
        "Date": "2007-12-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.900001525878906
      },
      {
        "Date": "2007-12-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.97999954223633
      },
      {
        "Date": "2007-12-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.33000183105469
      },
      {
        "Date": "2007-12-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.11000061035156
      },
      {
        "Date": "2007-12-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.83000183105469
      },
      {
        "Date": "2007-12-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.939998626708984
      },
      {
        "Date": "2007-12-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.63999938964844
      },
      {
        "Date": "2007-12-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.2599983215332
      },
      {
        "Date": "2007-12-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.650001525878906
      },
      {
        "Date": "2008-01-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.16999816894531
      },
      {
        "Date": "2008-01-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.880001068115234
      },
      {
        "Date": "2008-01-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.93000030517578
      },
      {
        "Date": "2008-01-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.34000015258789
      },
      {
        "Date": "2008-01-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.70000076293945
      },
      {
        "Date": "2008-01-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.2599983215332
      },
      {
        "Date": "2008-01-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.33000183105469
      },
      {
        "Date": "2008-01-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.86000061035156
      },
      {
        "Date": "2008-01-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.36000061035156
      },
      {
        "Date": "2008-01-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.16999816894531
      },
      {
        "Date": "2008-01-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.43000030517578
      },
      {
        "Date": "2008-01-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.040000915527344
      },
      {
        "Date": "2008-01-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.59000015258789
      },
      {
        "Date": "2008-01-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.86000061035156
      },
      {
        "Date": "2008-01-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.720001220703125
      },
      {
        "Date": "2008-01-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.959999084472656
      },
      {
        "Date": "2008-01-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.63999938964844
      },
      {
        "Date": "2008-01-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.56999969482422
      },
      {
        "Date": "2008-01-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.45000076293945
      },
      {
        "Date": "2008-01-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.349998474121094
      },
      {
        "Date": "2008-01-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.400001525878906
      },
      {"Date": "2008-02-01T00:00:00", "Bank": "JPM", "Stock Price": 48.25},
      {
        "Date": "2008-02-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.220001220703125
      },
      {
        "Date": "2008-02-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.88999938964844
      },
      {
        "Date": "2008-02-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.720001220703125
      },
      {
        "Date": "2008-02-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.11000061035156
      },
      {
        "Date": "2008-02-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.81999969482422
      },
      {
        "Date": "2008-02-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.349998474121094
      },
      {
        "Date": "2008-02-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.310001373291016
      },
      {
        "Date": "2008-02-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.099998474121094
      },
      {
        "Date": "2008-02-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.61000061035156
      },
      {"Date": "2008-02-15T00:00:00", "Bank": "JPM", "Stock Price": 43.25},
      {
        "Date": "2008-02-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.83000183105469
      },
      {
        "Date": "2008-02-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.150001525878906
      },
      {
        "Date": "2008-02-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.06999969482422
      },
      {
        "Date": "2008-02-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.93000030517578
      },
      {
        "Date": "2008-02-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.029998779296875
      },
      {
        "Date": "2008-02-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.720001220703125
      },
      {
        "Date": "2008-02-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.40999984741211
      },
      {
        "Date": "2008-02-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.439998626708984
      },
      {
        "Date": "2008-02-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.650001525878906
      },
      {
        "Date": "2008-03-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.81999969482422
      },
      {
        "Date": "2008-03-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.189998626708984
      },
      {
        "Date": "2008-03-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.7400016784668
      },
      {
        "Date": "2008-03-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.369998931884766
      },
      {
        "Date": "2008-03-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.560001373291016
      },
      {
        "Date": "2008-03-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.47999954223633
      },
      {
        "Date": "2008-03-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.84000015258789
      },
      {
        "Date": "2008-03-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.61000061035156
      },
      {
        "Date": "2008-03-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.11000061035156
      },
      {
        "Date": "2008-03-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.540000915527344
      },
      {
        "Date": "2008-03-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.310001373291016
      },
      {
        "Date": "2008-03-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.709999084472656
      },
      {
        "Date": "2008-03-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.470001220703125
      },
      {
        "Date": "2008-03-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.970001220703125
      },
      {
        "Date": "2008-03-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.54999923706055
      },
      {
        "Date": "2008-03-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.060001373291016
      },
      {
        "Date": "2008-03-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.11000061035156
      },
      {
        "Date": "2008-03-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.86000061035156
      },
      {
        "Date": "2008-03-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.709999084472656
      },
      {
        "Date": "2008-03-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.95000076293945
      },
      {"Date": "2008-04-01T00:00:00", "Bank": "JPM", "Stock Price": 47},
      {
        "Date": "2008-04-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.2400016784668
      },
      {
        "Date": "2008-04-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.279998779296875
      },
      {
        "Date": "2008-04-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.56999969482422
      },
      {
        "Date": "2008-04-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.540000915527344
      },
      {
        "Date": "2008-04-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.86000061035156
      },
      {
        "Date": "2008-04-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.29999923706055
      },
      {
        "Date": "2008-04-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.86000061035156
      },
      {
        "Date": "2008-04-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.529998779296875
      },
      {"Date": "2008-04-14T00:00:00", "Bank": "JPM", "Stock Price": 41.5},
      {
        "Date": "2008-04-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.119998931884766
      },
      {
        "Date": "2008-04-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.959999084472656
      },
      {
        "Date": "2008-04-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.119998931884766
      },
      {
        "Date": "2008-04-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.7599983215332
      },
      {
        "Date": "2008-04-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.22999954223633
      },
      {
        "Date": "2008-04-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.650001525878906
      },
      {
        "Date": "2008-04-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.150001525878906
      },
      {
        "Date": "2008-04-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.970001220703125
      },
      {
        "Date": "2008-04-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.790000915527344
      },
      {
        "Date": "2008-04-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.34000015258789
      },
      {
        "Date": "2008-04-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.08000183105469
      },
      {
        "Date": "2008-04-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.650001525878906
      },
      {"Date": "2008-05-01T00:00:00", "Bank": "JPM", "Stock Price": 49.25},
      {
        "Date": "2008-05-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.65999984741211
      },
      {"Date": "2008-05-05T00:00:00", "Bank": "JPM", "Stock Price": 48},
      {
        "Date": "2008-05-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.20000076293945
      },
      {
        "Date": "2008-05-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.56999969482422
      },
      {
        "Date": "2008-05-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.04999923706055
      },
      {
        "Date": "2008-05-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.56999969482422
      },
      {
        "Date": "2008-05-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.2400016784668
      },
      {
        "Date": "2008-05-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.47999954223633
      },
      {
        "Date": "2008-05-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.90999984741211
      },
      {
        "Date": "2008-05-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.02000045776367
      },
      {
        "Date": "2008-05-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.529998779296875
      },
      {
        "Date": "2008-05-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.9900016784668
      },
      {
        "Date": "2008-05-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.70000076293945
      },
      {
        "Date": "2008-05-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.41999816894531
      },
      {
        "Date": "2008-05-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.04999923706055
      },
      {
        "Date": "2008-05-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.31999969482422
      },
      {
        "Date": "2008-05-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.0099983215332
      },
      {
        "Date": "2008-05-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.86000061035156
      },
      {
        "Date": "2008-05-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.56999969482422
      },
      {"Date": "2008-05-30T00:00:00", "Bank": "JPM", "Stock Price": 43},
      {
        "Date": "2008-06-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.150001525878906
      },
      {
        "Date": "2008-06-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.88999938964844
      },
      {
        "Date": "2008-06-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.630001068115234
      },
      {
        "Date": "2008-06-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.099998474121094
      },
      {
        "Date": "2008-06-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.09000015258789
      },
      {
        "Date": "2008-06-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.5099983215332
      },
      {
        "Date": "2008-06-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.290000915527344
      },
      {
        "Date": "2008-06-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.130001068115234
      },
      {
        "Date": "2008-06-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.0099983215332
      },
      {
        "Date": "2008-06-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.58000183105469
      },
      {
        "Date": "2008-06-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.939998626708984
      },
      {
        "Date": "2008-06-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.040000915527344
      },
      {
        "Date": "2008-06-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.7400016784668
      },
      {
        "Date": "2008-06-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.650001525878906
      },
      {
        "Date": "2008-06-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.86000061035156
      },
      {
        "Date": "2008-06-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.869998931884766
      },
      {
        "Date": "2008-06-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.720001220703125
      },
      {
        "Date": "2008-06-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.90999984741211
      },
      {
        "Date": "2008-06-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.31999969482422
      },
      {
        "Date": "2008-06-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.04999923706055
      },
      {
        "Date": "2008-06-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.310001373291016
      },
      {
        "Date": "2008-07-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.02000045776367
      },
      {
        "Date": "2008-07-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.599998474121094
      },
      {
        "Date": "2008-07-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.310001373291016
      },
      {
        "Date": "2008-07-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.040000915527344
      },
      {
        "Date": "2008-07-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.77000045776367
      },
      {
        "Date": "2008-07-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.279998779296875
      },
      {
        "Date": "2008-07-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.5099983215332
      },
      {
        "Date": "2008-07-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.15999984741211
      },
      {
        "Date": "2008-07-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.690000534057617
      },
      {
        "Date": "2008-07-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.020000457763672
      },
      {
        "Date": "2008-07-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.939998626708984
      },
      {
        "Date": "2008-07-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.79999923706055
      },
      {
        "Date": "2008-07-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.02000045776367
      },
      {
        "Date": "2008-07-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.650001525878906
      },
      {
        "Date": "2008-07-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.86000061035156
      },
      {
        "Date": "2008-07-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.959999084472656
      },
      {
        "Date": "2008-07-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.13999938964844
      },
      {
        "Date": "2008-07-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.52000045776367
      },
      {
        "Date": "2008-07-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.65999984741211
      },
      {"Date": "2008-07-29T00:00:00", "Bank": "JPM", "Stock Price": 40.75},
      {
        "Date": "2008-07-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.56999969482422
      },
      {
        "Date": "2008-07-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.630001068115234
      },
      {
        "Date": "2008-08-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.7599983215332
      },
      {
        "Date": "2008-08-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.13999938964844
      },
      {
        "Date": "2008-08-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.88999938964844
      },
      {
        "Date": "2008-08-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.38999938964844
      },
      {
        "Date": "2008-08-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.810001373291016
      },
      {
        "Date": "2008-08-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.06999969482422
      },
      {
        "Date": "2008-08-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.88999938964844
      },
      {
        "Date": "2008-08-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.91999816894531
      },
      {
        "Date": "2008-08-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.90999984741211
      },
      {
        "Date": "2008-08-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.810001373291016
      },
      {
        "Date": "2008-08-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.06999969482422
      },
      {
        "Date": "2008-08-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.7400016784668
      },
      {
        "Date": "2008-08-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.58000183105469
      },
      {"Date": "2008-08-20T00:00:00", "Bank": "JPM", "Stock Price": 37},
      {
        "Date": "2008-08-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.2599983215332
      },
      {
        "Date": "2008-08-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.66999816894531
      },
      {
        "Date": "2008-08-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.130001068115234
      },
      {
        "Date": "2008-08-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.61000061035156
      },
      {
        "Date": "2008-08-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.13999938964844
      },
      {
        "Date": "2008-08-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.880001068115234
      },
      {
        "Date": "2008-08-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.4900016784668
      },
      {
        "Date": "2008-09-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.9900016784668
      },
      {
        "Date": "2008-09-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.709999084472656
      },
      {
        "Date": "2008-09-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.90999984741211
      },
      {
        "Date": "2008-09-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.599998474121094
      },
      {
        "Date": "2008-09-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.54999923706055
      },
      {
        "Date": "2008-09-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.470001220703125
      },
      {
        "Date": "2008-09-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.400001525878906
      },
      {
        "Date": "2008-09-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.650001525878906
      },
      {
        "Date": "2008-09-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.16999816894531
      },
      {"Date": "2008-09-15T00:00:00", "Bank": "JPM", "Stock Price": 37},
      {
        "Date": "2008-09-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.7400016784668
      },
      {
        "Date": "2008-09-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.77000045776367
      },
      {
        "Date": "2008-09-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.29999923706055
      },
      {
        "Date": "2008-09-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.04999923706055
      },
      {
        "Date": "2008-09-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.79999923706055
      },
      {
        "Date": "2008-09-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.560001373291016
      },
      {"Date": "2008-09-24T00:00:00", "Bank": "JPM", "Stock Price": 40.5},
      {
        "Date": "2008-09-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.459999084472656
      },
      {
        "Date": "2008-09-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 48.2400016784668
      },
      {"Date": "2008-09-29T00:00:00", "Bank": "JPM", "Stock Price": 41},
      {
        "Date": "2008-09-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.70000076293945
      },
      {
        "Date": "2008-10-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.630001068115234
      },
      {
        "Date": "2008-10-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 49.849998474121094
      },
      {
        "Date": "2008-10-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.900001525878906
      },
      {"Date": "2008-10-06T00:00:00", "Bank": "JPM", "Stock Price": 44},
      {
        "Date": "2008-10-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.31999969482422
      },
      {
        "Date": "2008-10-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.29999923706055
      },
      {
        "Date": "2008-10-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.68000030517578
      },
      {
        "Date": "2008-10-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.63999938964844
      },
      {
        "Date": "2008-10-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.9900016784668
      },
      {
        "Date": "2008-10-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.709999084472656
      },
      {
        "Date": "2008-10-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.4900016784668
      },
      {
        "Date": "2008-10-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.4900016784668
      },
      {
        "Date": "2008-10-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.33000183105469
      },
      {
        "Date": "2008-10-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.65999984741211
      },
      {
        "Date": "2008-10-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.7400016784668
      },
      {
        "Date": "2008-10-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.16999816894531
      },
      {
        "Date": "2008-10-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.849998474121094
      },
      {
        "Date": "2008-10-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.43000030517578
      },
      {"Date": "2008-10-27T00:00:00", "Bank": "JPM", "Stock Price": 34},
      {
        "Date": "2008-10-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.599998474121094
      },
      {
        "Date": "2008-10-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.709999084472656
      },
      {
        "Date": "2008-10-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.619998931884766
      },
      {"Date": "2008-10-31T00:00:00", "Bank": "JPM", "Stock Price": 41.25},
      {
        "Date": "2008-11-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.72999954223633
      },
      {
        "Date": "2008-11-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.16999816894531
      },
      {
        "Date": "2008-11-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.220001220703125
      },
      {
        "Date": "2008-11-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.2599983215332
      },
      {"Date": "2008-11-07T00:00:00", "Bank": "JPM", "Stock Price": 37.75},
      {
        "Date": "2008-11-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.40999984741211
      },
      {
        "Date": "2008-11-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.349998474121094
      },
      {
        "Date": "2008-11-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.56999969482422
      },
      {
        "Date": "2008-11-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.189998626708984
      },
      {
        "Date": "2008-11-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.470001220703125
      },
      {
        "Date": "2008-11-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.77000045776367
      },
      {
        "Date": "2008-11-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.13999938964844
      },
      {
        "Date": "2008-11-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.469999313354492
      },
      {
        "Date": "2008-11-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 23.3799991607666
      },
      {
        "Date": "2008-11-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 22.719999313354492
      },
      {
        "Date": "2008-11-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.579999923706055
      },
      {
        "Date": "2008-11-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.770000457763672
      },
      {
        "Date": "2008-11-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 30.6200008392334
      },
      {
        "Date": "2008-11-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.65999984741211
      },
      {
        "Date": "2008-12-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 26.1200008392334
      },
      {
        "Date": "2008-12-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.530000686645508
      },
      {"Date": "2008-12-03T00:00:00", "Bank": "JPM", "Stock Price": 30.25},
      {
        "Date": "2008-12-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.079999923706055
      },
      {
        "Date": "2008-12-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.349998474121094
      },
      {
        "Date": "2008-12-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.4900016784668
      },
      {
        "Date": "2008-12-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.959999084472656
      },
      {
        "Date": "2008-12-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.52000045776367
      },
      {
        "Date": "2008-12-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.940000534057617
      },
      {
        "Date": "2008-12-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 30.940000534057617
      },
      {
        "Date": "2008-12-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.6299991607666
      },
      {
        "Date": "2008-12-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.349998474121094
      },
      {
        "Date": "2008-12-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.860000610351562
      },
      {
        "Date": "2008-12-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 30.209999084472656
      },
      {
        "Date": "2008-12-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 30.31999969482422
      },
      {
        "Date": "2008-12-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.81999969482422
      },
      {
        "Date": "2008-12-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.110000610351562
      },
      {
        "Date": "2008-12-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.850000381469727
      },
      {
        "Date": "2008-12-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.799999237060547
      },
      {
        "Date": "2008-12-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.780000686645508
      },
      {
        "Date": "2008-12-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.010000228881836
      },
      {
        "Date": "2008-12-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.530000686645508
      },
      {
        "Date": "2009-01-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.350000381469727
      },
      {"Date": "2009-01-05T00:00:00", "Bank": "JPM", "Stock Price": 29.25},
      {
        "Date": "2009-01-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.8799991607666
      },
      {
        "Date": "2009-01-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.09000015258789
      },
      {
        "Date": "2009-01-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.219999313354492
      },
      {
        "Date": "2009-01-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 25.969999313354492
      },
      {
        "Date": "2009-01-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.90999984741211
      },
      {
        "Date": "2009-01-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 26.350000381469727
      },
      {
        "Date": "2009-01-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 25.90999984741211
      },
      {
        "Date": "2009-01-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.34000015258789
      },
      {
        "Date": "2009-01-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 22.81999969482422
      },
      {
        "Date": "2009-01-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 18.09000015258789
      },
      {
        "Date": "2009-01-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 22.6299991607666
      },
      {
        "Date": "2009-01-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 23.100000381469727
      },
      {
        "Date": "2009-01-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.280000686645508
      },
      {"Date": "2009-01-26T00:00:00", "Bank": "JPM", "Stock Price": 24.5},
      {
        "Date": "2009-01-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 25.059999465942383
      },
      {
        "Date": "2009-01-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.65999984741211
      },
      {
        "Date": "2009-01-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 25.43000030517578
      },
      {
        "Date": "2009-01-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 25.510000228881836
      },
      {
        "Date": "2009-02-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 25.200000762939453
      },
      {
        "Date": "2009-02-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.049999237060547
      },
      {
        "Date": "2009-02-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.040000915527344
      },
      {
        "Date": "2009-02-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.540000915527344
      },
      {
        "Date": "2009-02-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.6299991607666
      },
      {
        "Date": "2009-02-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.280000686645508
      },
      {
        "Date": "2009-02-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.6200008392334
      },
      {
        "Date": "2009-02-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 26.09000015258789
      },
      {
        "Date": "2009-02-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 26.190000534057617
      },
      {
        "Date": "2009-02-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.690000534057617
      },
      {
        "Date": "2009-02-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 21.649999618530273
      },
      {
        "Date": "2009-02-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 21.510000228881836
      },
      {
        "Date": "2009-02-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 20.600000381469727
      },
      {
        "Date": "2009-02-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 19.899999618530273
      },
      {
        "Date": "2009-02-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 19.510000228881836
      },
      {
        "Date": "2009-02-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 21.020000457763672
      },
      {
        "Date": "2009-02-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 21.729999542236328
      },
      {
        "Date": "2009-02-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 23.049999237060547
      },
      {
        "Date": "2009-02-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 22.850000381469727
      },
      {
        "Date": "2009-03-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 21.15999984741211
      },
      {
        "Date": "2009-03-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 21.010000228881836
      },
      {
        "Date": "2009-03-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 19.299999237060547
      },
      {
        "Date": "2009-03-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 16.600000381469727
      },
      {
        "Date": "2009-03-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 15.930000305175781
      },
      {
        "Date": "2009-03-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 15.899999618530273
      },
      {"Date": "2009-03-10T00:00:00", "Bank": "JPM", "Stock Price": 19.5},
      {
        "Date": "2009-03-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 20.399999618530273
      },
      {
        "Date": "2009-03-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 23.200000762939453
      },
      {"Date": "2009-03-13T00:00:00", "Bank": "JPM", "Stock Price": 23.75},
      {
        "Date": "2009-03-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 23.09000015258789
      },
      {
        "Date": "2009-03-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 25.139999389648438
      },
      {
        "Date": "2009-03-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.110000610351562
      },
      {
        "Date": "2009-03-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.950000762939453
      },
      {
        "Date": "2009-03-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 23.149999618530273
      },
      {
        "Date": "2009-03-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.860000610351562
      },
      {
        "Date": "2009-03-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 26.399999618530273
      },
      {
        "Date": "2009-03-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.559999465942383
      },
      {
        "Date": "2009-03-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.100000381469727
      },
      {
        "Date": "2009-03-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.399999618530273
      },
      {
        "Date": "2009-03-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 24.850000381469727
      },
      {
        "Date": "2009-03-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 26.579999923706055
      },
      {
        "Date": "2009-04-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.139999389648438
      },
      {
        "Date": "2009-04-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.15999984741211
      },
      {
        "Date": "2009-04-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.280000686645508
      },
      {
        "Date": "2009-04-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 28.200000762939453
      },
      {"Date": "2009-04-07T00:00:00", "Bank": "JPM", "Stock Price": 27.25},
      {
        "Date": "2009-04-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 27.43000030517578
      },
      {"Date": "2009-04-09T00:00:00", "Bank": "JPM", "Stock Price": 32.75},
      {
        "Date": "2009-04-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.70000076293945
      },
      {
        "Date": "2009-04-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 30.700000762939453
      },
      {
        "Date": "2009-04-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.560001373291016
      },
      {
        "Date": "2009-04-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.2400016784668
      },
      {
        "Date": "2009-04-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.2599983215332
      },
      {
        "Date": "2009-04-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 29.690000534057617
      },
      {
        "Date": "2009-04-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.529998779296875
      },
      {
        "Date": "2009-04-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 31.899999618530273
      },
      {
        "Date": "2009-04-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.209999084472656
      },
      {
        "Date": "2009-04-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.380001068115234
      },
      {
        "Date": "2009-04-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.779998779296875
      },
      {
        "Date": "2009-04-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.790000915527344
      },
      {
        "Date": "2009-04-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.47999954223633
      },
      {"Date": "2009-04-30T00:00:00", "Bank": "JPM", "Stock Price": 33},
      {
        "Date": "2009-05-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.4900016784668
      },
      {
        "Date": "2009-05-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.790000915527344
      },
      {
        "Date": "2009-05-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.81999969482422
      },
      {
        "Date": "2009-05-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.220001220703125
      },
      {
        "Date": "2009-05-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.2400016784668
      },
      {
        "Date": "2009-05-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.939998626708984
      },
      {
        "Date": "2009-05-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.83000183105469
      },
      {
        "Date": "2009-05-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.36000061035156
      },
      {
        "Date": "2009-05-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.04999923706055
      },
      {
        "Date": "2009-05-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.540000915527344
      },
      {
        "Date": "2009-05-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.90999984741211
      },
      {
        "Date": "2009-05-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.2599983215332
      },
      {
        "Date": "2009-05-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.810001373291016
      },
      {
        "Date": "2009-05-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.54999923706055
      },
      {
        "Date": "2009-05-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.900001525878906
      },
      {
        "Date": "2009-05-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.40999984741211
      },
      {
        "Date": "2009-05-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.540000915527344
      },
      {
        "Date": "2009-05-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.65999984741211
      },
      {
        "Date": "2009-05-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.650001525878906
      },
      {
        "Date": "2009-05-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.900001525878906
      },
      {
        "Date": "2009-06-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.11000061035156
      },
      {"Date": "2009-06-02T00:00:00", "Bank": "JPM", "Stock Price": 34.5},
      {
        "Date": "2009-06-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.97999954223633
      },
      {
        "Date": "2009-06-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.349998474121094
      },
      {
        "Date": "2009-06-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.54999923706055
      },
      {
        "Date": "2009-06-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.38999938964844
      },
      {
        "Date": "2009-06-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.2599983215332
      },
      {
        "Date": "2009-06-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.84000015258789
      },
      {
        "Date": "2009-06-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.939998626708984
      },
      {
        "Date": "2009-06-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.130001068115234
      },
      {"Date": "2009-06-15T00:00:00", "Bank": "JPM", "Stock Price": 34},
      {"Date": "2009-06-16T00:00:00", "Bank": "JPM", "Stock Price": 33.5},
      {
        "Date": "2009-06-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.72999954223633
      },
      {
        "Date": "2009-06-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.16999816894531
      },
      {"Date": "2009-06-19T00:00:00", "Bank": "JPM", "Stock Price": 35},
      {
        "Date": "2009-06-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.869998931884766
      },
      {
        "Date": "2009-06-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.56999969482422
      },
      {
        "Date": "2009-06-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.459999084472656
      },
      {
        "Date": "2009-06-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.13999938964844
      },
      {
        "Date": "2009-06-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.45000076293945
      },
      {
        "Date": "2009-06-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.599998474121094
      },
      {
        "Date": "2009-06-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.11000061035156
      },
      {
        "Date": "2009-07-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.77000045776367
      },
      {
        "Date": "2009-07-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.27000045776367
      },
      {
        "Date": "2009-07-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.599998474121094
      },
      {
        "Date": "2009-07-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.810001373291016
      },
      {
        "Date": "2009-07-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.709999084472656
      },
      {
        "Date": "2009-07-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 33.619998931884766
      },
      {
        "Date": "2009-07-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 32.34000015258789
      },
      {
        "Date": "2009-07-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.709999084472656
      },
      {
        "Date": "2009-07-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 34.70000076293945
      },
      {
        "Date": "2009-07-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.2599983215332
      },
      {
        "Date": "2009-07-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.130001068115234
      },
      {
        "Date": "2009-07-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.88999938964844
      },
      {
        "Date": "2009-07-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.97999954223633
      },
      {
        "Date": "2009-07-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.939998626708984
      },
      {
        "Date": "2009-07-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.83000183105469
      },
      {
        "Date": "2009-07-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.150001525878906
      },
      {
        "Date": "2009-07-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.91999816894531
      },
      {
        "Date": "2009-07-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.130001068115234
      },
      {
        "Date": "2009-07-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.08000183105469
      },
      {
        "Date": "2009-07-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.77000045776367
      },
      {
        "Date": "2009-07-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.470001220703125
      },
      {
        "Date": "2009-07-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.650001525878906
      },
      {
        "Date": "2009-08-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.599998474121094
      },
      {
        "Date": "2009-08-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.209999084472656
      },
      {
        "Date": "2009-08-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.779998779296875
      },
      {"Date": "2009-08-06T00:00:00", "Bank": "JPM", "Stock Price": 40.75},
      {
        "Date": "2009-08-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.36000061035156
      },
      {
        "Date": "2009-08-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.689998626708984
      },
      {
        "Date": "2009-08-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.2400016784668
      },
      {
        "Date": "2009-08-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.209999084472656
      },
      {
        "Date": "2009-08-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.900001525878906
      },
      {
        "Date": "2009-08-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.45000076293945
      },
      {
        "Date": "2009-08-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.72999954223633
      },
      {
        "Date": "2009-08-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.70000076293945
      },
      {
        "Date": "2009-08-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.40999984741211
      },
      {
        "Date": "2009-08-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.41999816894531
      },
      {
        "Date": "2009-08-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.65999984741211
      },
      {
        "Date": "2009-08-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.0099983215332
      },
      {
        "Date": "2009-08-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.58000183105469
      },
      {
        "Date": "2009-08-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.29999923706055
      },
      {
        "Date": "2009-08-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.45000076293945
      },
      {
        "Date": "2009-08-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.91999816894531
      },
      {
        "Date": "2009-08-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.459999084472656
      },
      {
        "Date": "2009-09-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.66999816894531
      },
      {
        "Date": "2009-09-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.86000061035156
      },
      {
        "Date": "2009-09-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.11000061035156
      },
      {
        "Date": "2009-09-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.34000015258789
      },
      {
        "Date": "2009-09-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.540000915527344
      },
      {
        "Date": "2009-09-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.86000061035156
      },
      {
        "Date": "2009-09-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.02000045776367
      },
      {"Date": "2009-09-11T00:00:00", "Bank": "JPM", "Stock Price": 42.5},
      {"Date": "2009-09-14T00:00:00", "Bank": "JPM", "Stock Price": 43.75},
      {
        "Date": "2009-09-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.189998626708984
      },
      {
        "Date": "2009-09-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.650001525878906
      },
      {
        "Date": "2009-09-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.959999084472656
      },
      {
        "Date": "2009-09-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.95000076293945
      },
      {
        "Date": "2009-09-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.54999923706055
      },
      {
        "Date": "2009-09-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.470001220703125
      },
      {
        "Date": "2009-09-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.060001373291016
      },
      {
        "Date": "2009-09-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.369998931884766
      },
      {
        "Date": "2009-09-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.650001525878906
      },
      {
        "Date": "2009-09-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.810001373291016
      },
      {
        "Date": "2009-09-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.880001068115234
      },
      {
        "Date": "2009-09-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.81999969482422
      },
      {
        "Date": "2009-10-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.369998931884766
      },
      {
        "Date": "2009-10-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.86000061035156
      },
      {
        "Date": "2009-10-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.79999923706055
      },
      {
        "Date": "2009-10-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.90999984741211
      },
      {
        "Date": "2009-10-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.70000076293945
      },
      {
        "Date": "2009-10-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.29999923706055
      },
      {
        "Date": "2009-10-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.849998474121094
      },
      {
        "Date": "2009-10-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.08000183105469
      },
      {
        "Date": "2009-10-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.65999984741211
      },
      {
        "Date": "2009-10-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.15999984741211
      },
      {
        "Date": "2009-10-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.15999984741211
      },
      {
        "Date": "2009-10-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.060001373291016
      },
      {
        "Date": "2009-10-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.97999954223633
      },
      {
        "Date": "2009-10-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.029998779296875
      },
      {
        "Date": "2009-10-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.650001525878906
      },
      {
        "Date": "2009-10-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.709999084472656
      },
      {
        "Date": "2009-10-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.22999954223633
      },
      {
        "Date": "2009-10-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.81999969482422
      },
      {
        "Date": "2009-10-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.900001525878906
      },
      {
        "Date": "2009-10-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.68000030517578
      },
      {
        "Date": "2009-10-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.349998474121094
      },
      {
        "Date": "2009-10-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.77000045776367
      },
      {
        "Date": "2009-11-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.58000183105469
      },
      {
        "Date": "2009-11-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.70000076293945
      },
      {
        "Date": "2009-11-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.209999084472656
      },
      {
        "Date": "2009-11-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.869998931884766
      },
      {
        "Date": "2009-11-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.47999954223633
      },
      {
        "Date": "2009-11-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.349998474121094
      },
      {
        "Date": "2009-11-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.16999816894531
      },
      {
        "Date": "2009-11-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.31999969482422
      },
      {
        "Date": "2009-11-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.29999923706055
      },
      {
        "Date": "2009-11-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.900001525878906
      },
      {
        "Date": "2009-11-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.040000915527344
      },
      {
        "Date": "2009-11-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.15999984741211
      },
      {
        "Date": "2009-11-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.380001068115234
      },
      {
        "Date": "2009-11-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.54999923706055
      },
      {
        "Date": "2009-11-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.459999084472656
      },
      {
        "Date": "2009-11-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.279998779296875
      },
      {
        "Date": "2009-11-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.47999954223633
      },
      {
        "Date": "2009-11-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.15999984741211
      },
      {
        "Date": "2009-11-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.33000183105469
      },
      {
        "Date": "2009-11-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.4900016784668
      },
      {
        "Date": "2009-12-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.220001220703125
      },
      {
        "Date": "2009-12-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.93000030517578
      },
      {
        "Date": "2009-12-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.400001525878906
      },
      {
        "Date": "2009-12-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.7400016784668
      },
      {"Date": "2009-12-07T00:00:00", "Bank": "JPM", "Stock Price": 41.25},
      {
        "Date": "2009-12-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.209999084472656
      },
      {
        "Date": "2009-12-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.189998626708984
      },
      {
        "Date": "2009-12-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.27000045776367
      },
      {
        "Date": "2009-12-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.959999084472656
      },
      {
        "Date": "2009-12-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.77000045776367
      },
      {
        "Date": "2009-12-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.86000061035156
      },
      {
        "Date": "2009-12-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.36000061035156
      },
      {
        "Date": "2009-12-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.27000045776367
      },
      {
        "Date": "2009-12-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.95000076293945
      },
      {
        "Date": "2009-12-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.900001525878906
      },
      {
        "Date": "2009-12-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.939998626708984
      },
      {
        "Date": "2009-12-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.560001373291016
      },
      {
        "Date": "2009-12-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.88999938964844
      },
      {
        "Date": "2009-12-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.720001220703125
      },
      {
        "Date": "2009-12-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.4900016784668
      },
      {
        "Date": "2009-12-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.529998779296875
      },
      {
        "Date": "2009-12-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.66999816894531
      },
      {
        "Date": "2010-01-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.849998474121094
      },
      {
        "Date": "2010-01-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.68000030517578
      },
      {
        "Date": "2010-01-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.91999816894531
      },
      {
        "Date": "2010-01-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.790000915527344
      },
      {
        "Date": "2010-01-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.68000030517578
      },
      {
        "Date": "2010-01-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.529998779296875
      },
      {
        "Date": "2010-01-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.4900016784668
      },
      {"Date": "2010-01-13T00:00:00", "Bank": "JPM", "Stock Price": 44.25},
      {
        "Date": "2010-01-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.689998626708984
      },
      {
        "Date": "2010-01-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.68000030517578
      },
      {
        "Date": "2010-01-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.279998779296875
      },
      {
        "Date": "2010-01-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.400001525878906
      },
      {
        "Date": "2010-01-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.540000915527344
      },
      {
        "Date": "2010-01-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.15999984741211
      },
      {
        "Date": "2010-01-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.209999084472656
      },
      {
        "Date": "2010-01-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.439998626708984
      },
      {
        "Date": "2010-01-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.33000183105469
      },
      {
        "Date": "2010-01-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.47999954223633
      },
      {
        "Date": "2010-01-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.939998626708984
      },
      {
        "Date": "2010-02-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.630001068115234
      },
      {
        "Date": "2010-02-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.54999923706055
      },
      {
        "Date": "2010-02-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.290000915527344
      },
      {
        "Date": "2010-02-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.349998474121094
      },
      {
        "Date": "2010-02-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.29999923706055
      },
      {
        "Date": "2010-02-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.70000076293945
      },
      {
        "Date": "2010-02-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.38999938964844
      },
      {
        "Date": "2010-02-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.869998931884766
      },
      {
        "Date": "2010-02-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.02000045776367
      },
      {
        "Date": "2010-02-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.95000076293945
      },
      {
        "Date": "2010-02-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.06999969482422
      },
      {
        "Date": "2010-02-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.040000915527344
      },
      {
        "Date": "2010-02-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.40999984741211
      },
      {
        "Date": "2010-02-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.029998779296875
      },
      {
        "Date": "2010-02-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.849998474121094
      },
      {
        "Date": "2010-02-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.880001068115234
      },
      {
        "Date": "2010-02-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.849998474121094
      },
      {
        "Date": "2010-02-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.63999938964844
      },
      {
        "Date": "2010-02-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.970001220703125
      },
      {
        "Date": "2010-03-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.83000183105469
      },
      {
        "Date": "2010-03-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.619998931884766
      },
      {
        "Date": "2010-03-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.529998779296875
      },
      {
        "Date": "2010-03-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.91999816894531
      },
      {
        "Date": "2010-03-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.810001373291016
      },
      {
        "Date": "2010-03-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.59000015258789
      },
      {
        "Date": "2010-03-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.41999816894531
      },
      {
        "Date": "2010-03-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.93000030517578
      },
      {
        "Date": "2010-03-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.18000030517578
      },
      {
        "Date": "2010-03-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.150001525878906
      },
      {
        "Date": "2010-03-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.06999969482422
      },
      {
        "Date": "2010-03-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.2400016784668
      },
      {
        "Date": "2010-03-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.790000915527344
      },
      {
        "Date": "2010-03-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.63999938964844
      },
      {
        "Date": "2010-03-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.45000076293945
      },
      {
        "Date": "2010-03-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.7400016784668
      },
      {
        "Date": "2010-03-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.58000183105469
      },
      {
        "Date": "2010-03-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.939998626708984
      },
      {
        "Date": "2010-03-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.939998626708984
      },
      {
        "Date": "2010-03-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.02000045776367
      },
      {
        "Date": "2010-03-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.86000061035156
      },
      {
        "Date": "2010-03-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.58000183105469
      },
      {"Date": "2010-03-31T00:00:00", "Bank": "JPM", "Stock Price": 44.75},
      {
        "Date": "2010-04-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.18000030517578
      },
      {
        "Date": "2010-04-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.34000015258789
      },
      {
        "Date": "2010-04-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.84000015258789
      },
      {
        "Date": "2010-04-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.31999969482422
      },
      {
        "Date": "2010-04-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.7599983215332
      },
      {
        "Date": "2010-04-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.97999954223633
      },
      {
        "Date": "2010-04-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 46.13999938964844
      },
      {
        "Date": "2010-04-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.869998931884766
      },
      {
        "Date": "2010-04-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.72999954223633
      },
      {
        "Date": "2010-04-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 47.810001373291016
      },
      {
        "Date": "2010-04-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.54999923706055
      },
      {
        "Date": "2010-04-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.38999938964844
      },
      {
        "Date": "2010-04-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.880001068115234
      },
      {
        "Date": "2010-04-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 45.349998474121094
      },
      {
        "Date": "2010-04-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.7400016784668
      },
      {
        "Date": "2010-04-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 44.939998626708984
      },
      {
        "Date": "2010-04-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.88999938964844
      },
      {
        "Date": "2010-04-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.40999984741211
      },
      {
        "Date": "2010-04-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.459999084472656
      },
      {"Date": "2010-04-29T00:00:00", "Bank": "JPM", "Stock Price": 44},
      {
        "Date": "2010-04-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.58000183105469
      },
      {
        "Date": "2010-05-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 43.529998779296875
      },
      {
        "Date": "2010-05-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.470001220703125
      },
      {
        "Date": "2010-05-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.630001068115234
      },
      {
        "Date": "2010-05-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.810001373291016
      },
      {
        "Date": "2010-05-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.7599983215332
      },
      {
        "Date": "2010-05-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.95000076293945
      },
      {
        "Date": "2010-05-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.54999923706055
      },
      {
        "Date": "2010-05-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.689998626708984
      },
      {
        "Date": "2010-05-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.810001373291016
      },
      {
        "Date": "2010-05-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.88999938964844
      },
      {
        "Date": "2010-05-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.84000015258789
      },
      {
        "Date": "2010-05-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.02000045776367
      },
      {
        "Date": "2010-05-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.380001068115234
      },
      {
        "Date": "2010-05-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.83000183105469
      },
      {
        "Date": "2010-05-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.04999923706055
      },
      {
        "Date": "2010-05-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.619998931884766
      },
      {
        "Date": "2010-05-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.939998626708984
      },
      {
        "Date": "2010-05-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.779998779296875
      },
      {
        "Date": "2010-05-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.41999816894531
      },
      {
        "Date": "2010-05-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.58000183105469
      },
      {
        "Date": "2010-06-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.540000915527344
      },
      {
        "Date": "2010-06-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.54999923706055
      },
      {
        "Date": "2010-06-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.099998474121094
      },
      {
        "Date": "2010-06-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.619998931884766
      },
      {
        "Date": "2010-06-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.720001220703125
      },
      {
        "Date": "2010-06-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.779998779296875
      },
      {
        "Date": "2010-06-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.119998931884766
      },
      {
        "Date": "2010-06-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.290000915527344
      },
      {
        "Date": "2010-06-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.09000015258789
      },
      {
        "Date": "2010-06-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.33000183105469
      },
      {"Date": "2010-06-15T00:00:00", "Bank": "JPM", "Stock Price": 38.25},
      {
        "Date": "2010-06-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.52000045776367
      },
      {
        "Date": "2010-06-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.439998626708984
      },
      {
        "Date": "2010-06-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.18000030517578
      },
      {
        "Date": "2010-06-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.869998931884766
      },
      {
        "Date": "2010-06-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.33000183105469
      },
      {
        "Date": "2010-06-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.88999938964844
      },
      {
        "Date": "2010-06-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.029998779296875
      },
      {
        "Date": "2010-06-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.439998626708984
      },
      {
        "Date": "2010-06-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.540000915527344
      },
      {
        "Date": "2010-06-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.060001373291016
      },
      {
        "Date": "2010-06-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.61000061035156
      },
      {
        "Date": "2010-07-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.08000183105469
      },
      {
        "Date": "2010-07-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.83000183105469
      },
      {
        "Date": "2010-07-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.33000183105469
      },
      {
        "Date": "2010-07-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.150001525878906
      },
      {
        "Date": "2010-07-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.15999984741211
      },
      {
        "Date": "2010-07-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.849998474121094
      },
      {
        "Date": "2010-07-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.189998626708984
      },
      {
        "Date": "2010-07-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.47999954223633
      },
      {
        "Date": "2010-07-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.349998474121094
      },
      {
        "Date": "2010-07-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.459999084472656
      },
      {"Date": "2010-07-16T00:00:00", "Bank": "JPM", "Stock Price": 39},
      {
        "Date": "2010-07-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.040000915527344
      },
      {
        "Date": "2010-07-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.630001068115234
      },
      {
        "Date": "2010-07-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.41999816894531
      },
      {
        "Date": "2010-07-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.349998474121094
      },
      {
        "Date": "2010-07-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.83000183105469
      },
      {
        "Date": "2010-07-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.33000183105469
      },
      {
        "Date": "2010-07-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.689998626708984
      },
      {
        "Date": "2010-07-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.31999969482422
      },
      {
        "Date": "2010-07-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.209999084472656
      },
      {
        "Date": "2010-07-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.279998779296875
      },
      {
        "Date": "2010-08-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.63999938964844
      },
      {
        "Date": "2010-08-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.08000183105469
      },
      {
        "Date": "2010-08-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.290000915527344
      },
      {
        "Date": "2010-08-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.27000045776367
      },
      {
        "Date": "2010-08-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.439998626708984
      },
      {
        "Date": "2010-08-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.81999969482422
      },
      {
        "Date": "2010-08-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.16999816894531
      },
      {
        "Date": "2010-08-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.77000045776367
      },
      {
        "Date": "2010-08-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.810001373291016
      },
      {"Date": "2010-08-13T00:00:00", "Bank": "JPM", "Stock Price": 37.5},
      {
        "Date": "2010-08-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.689998626708984
      },
      {
        "Date": "2010-08-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.47999954223633
      },
      {
        "Date": "2010-08-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.88999938964844
      },
      {
        "Date": "2010-08-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.06999969482422
      },
      {
        "Date": "2010-08-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.13999938964844
      },
      {
        "Date": "2010-08-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.880001068115234
      },
      {
        "Date": "2010-08-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.209999084472656
      },
      {
        "Date": "2010-08-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.22999954223633
      },
      {
        "Date": "2010-08-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.630001068115234
      },
      {
        "Date": "2010-08-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.599998474121094
      },
      {
        "Date": "2010-08-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 35.849998474121094
      },
      {
        "Date": "2010-08-31T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.36000061035156
      },
      {
        "Date": "2010-09-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.7400016784668
      },
      {
        "Date": "2010-09-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.15999984741211
      },
      {
        "Date": "2010-09-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.16999816894531
      },
      {
        "Date": "2010-09-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.279998779296875
      },
      {
        "Date": "2010-09-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.119998931884766
      },
      {
        "Date": "2010-09-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.099998474121094
      },
      {
        "Date": "2010-09-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.7599983215332
      },
      {
        "Date": "2010-09-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.119998931884766
      },
      {
        "Date": "2010-09-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.720001220703125
      },
      {
        "Date": "2010-09-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.97999954223633
      },
      {
        "Date": "2010-09-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.9900016784668
      },
      {
        "Date": "2010-09-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.060001373291016
      },
      {
        "Date": "2010-09-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.189998626708984
      },
      {
        "Date": "2010-09-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.59000015258789
      },
      {
        "Date": "2010-09-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.939998626708984
      },
      {
        "Date": "2010-09-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.099998474121094
      },
      {"Date": "2010-09-24T00:00:00", "Bank": "JPM", "Stock Price": 39.75},
      {
        "Date": "2010-09-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.08000183105469
      },
      {
        "Date": "2010-09-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.95000076293945
      },
      {
        "Date": "2010-09-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.40999984741211
      },
      {
        "Date": "2010-09-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.060001373291016
      },
      {
        "Date": "2010-10-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.810001373291016
      },
      {
        "Date": "2010-10-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.95000076293945
      },
      {
        "Date": "2010-10-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.63999938964844
      },
      {
        "Date": "2010-10-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2010-10-07T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.52000045776367
      },
      {
        "Date": "2010-10-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.310001373291016
      },
      {
        "Date": "2010-10-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.72999954223633
      },
      {
        "Date": "2010-10-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.400001525878906
      },
      {
        "Date": "2010-10-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.84000015258789
      },
      {
        "Date": "2010-10-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.720001220703125
      },
      {
        "Date": "2010-10-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.150001525878906
      },
      {
        "Date": "2010-10-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.20000076293945
      },
      {
        "Date": "2010-10-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.689998626708984
      },
      {
        "Date": "2010-10-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.099998474121094
      },
      {
        "Date": "2010-10-21T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.70000076293945
      },
      {
        "Date": "2010-10-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.70000076293945
      },
      {
        "Date": "2010-10-25T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.06999969482422
      },
      {
        "Date": "2010-10-26T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.20000076293945
      },
      {
        "Date": "2010-10-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.540000915527344
      },
      {
        "Date": "2010-10-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.5099983215332
      },
      {
        "Date": "2010-10-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.630001068115234
      },
      {
        "Date": "2010-11-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.41999816894531
      },
      {
        "Date": "2010-11-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 36.959999084472656
      },
      {
        "Date": "2010-11-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.720001220703125
      },
      {
        "Date": "2010-11-04T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.79999923706055
      },
      {
        "Date": "2010-11-05T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.939998626708984
      },
      {
        "Date": "2010-11-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.5099983215332
      },
      {
        "Date": "2010-11-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.900001525878906
      },
      {
        "Date": "2010-11-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.619998931884766
      },
      {
        "Date": "2010-11-11T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.02000045776367
      },
      {
        "Date": "2010-11-12T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.61000061035156
      },
      {
        "Date": "2010-11-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.08000183105469
      },
      {
        "Date": "2010-11-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.61000061035156
      },
      {
        "Date": "2010-11-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.18000030517578
      },
      {
        "Date": "2010-11-18T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.65999984741211
      },
      {
        "Date": "2010-11-19T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.40999984741211
      },
      {
        "Date": "2010-11-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.5099983215332
      },
      {
        "Date": "2010-11-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.630001068115234
      },
      {
        "Date": "2010-11-24T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.15999984741211
      },
      {"Date": "2010-11-26T00:00:00", "Bank": "JPM", "Stock Price": 37.5},
      {
        "Date": "2010-11-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.90999984741211
      },
      {
        "Date": "2010-11-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 37.400001525878906
      },
      {
        "Date": "2010-12-01T00:00:00",
        "Bank": "JPM",
        "Stock Price": 38.150001525878906
      },
      {
        "Date": "2010-12-02T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.310001373291016
      },
      {
        "Date": "2010-12-03T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.61000061035156
      },
      {
        "Date": "2010-12-06T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.900001525878906
      },
      {"Date": "2010-12-07T00:00:00", "Bank": "JPM", "Stock Price": 39.25},
      {
        "Date": "2010-12-08T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.2599983215332
      },
      {
        "Date": "2010-12-09T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.810001373291016
      },
      {
        "Date": "2010-12-10T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.43000030517578
      },
      {
        "Date": "2010-12-13T00:00:00",
        "Bank": "JPM",
        "Stock Price": 41.5099983215332
      },
      {
        "Date": "2010-12-14T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.790000915527344
      },
      {
        "Date": "2010-12-15T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.209999084472656
      },
      {
        "Date": "2010-12-16T00:00:00",
        "Bank": "JPM",
        "Stock Price": 40.0099983215332
      },
      {
        "Date": "2010-12-17T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.66999816894531
      },
      {
        "Date": "2010-12-20T00:00:00",
        "Bank": "JPM",
        "Stock Price": 39.95000076293945
      },
      {"Date": "2010-12-21T00:00:00", "Bank": "JPM", "Stock Price": 41},
      {
        "Date": "2010-12-22T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.15999984741211
      },
      {
        "Date": "2010-12-23T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.08000183105469
      },
      {
        "Date": "2010-12-27T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.66999816894531
      },
      {
        "Date": "2010-12-28T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.61000061035156
      },
      {
        "Date": "2010-12-29T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.36000061035156
      },
      {
        "Date": "2010-12-30T00:00:00",
        "Bank": "JPM",
        "Stock Price": 42.22999954223633
      },
      {
        "Date": "2007-01-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.62000274658203
      },
      {
        "Date": "2007-01-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.91000366210938
      },
      {
        "Date": "2007-01-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.86000061035156
      },
      {
        "Date": "2007-01-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.3499984741211
      },
      {
        "Date": "2007-01-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.16000366210938
      },
      {
        "Date": "2007-01-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.56999969482422
      },
      {
        "Date": "2007-01-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.37000274658203
      },
      {
        "Date": "2007-01-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.86000061035156
      },
      {
        "Date": "2007-01-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.61000061035156
      },
      {
        "Date": "2007-01-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.37999725341797
      },
      {
        "Date": "2007-01-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.20999908447266
      },
      {"Date": "2007-01-19T00:00:00", "Bank": "MS", "Stock Price": 81.5},
      {
        "Date": "2007-01-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.30999755859375
      },
      {
        "Date": "2007-01-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.62000274658203
      },
      {
        "Date": "2007-01-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.6500015258789
      },
      {
        "Date": "2007-01-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.22000122070312
      },
      {
        "Date": "2007-01-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.12000274658203
      },
      {
        "Date": "2007-01-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.12000274658203
      },
      {
        "Date": "2007-01-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.72000122070312
      },
      {
        "Date": "2007-01-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.79000091552734
      },
      {
        "Date": "2007-02-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.8499984741211
      },
      {
        "Date": "2007-02-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.04000091552734
      },
      {
        "Date": "2007-02-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.2699966430664
      },
      {
        "Date": "2007-02-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.12999725341797
      },
      {
        "Date": "2007-02-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.23999786376953
      },
      {
        "Date": "2007-02-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.81999969482422
      },
      {
        "Date": "2007-02-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.77999877929688
      },
      {
        "Date": "2007-02-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.27999877929688
      },
      {"Date": "2007-02-13T00:00:00", "Bank": "MS", "Stock Price": 81.25},
      {
        "Date": "2007-02-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.36000061035156
      },
      {
        "Date": "2007-02-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.81999969482422
      },
      {
        "Date": "2007-02-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.36000061035156
      },
      {
        "Date": "2007-02-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.30999755859375
      },
      {
        "Date": "2007-02-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.19000244140625
      },
      {"Date": "2007-02-22T00:00:00", "Bank": "MS", "Stock Price": 82.75},
      {
        "Date": "2007-02-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.97000122070312
      },
      {
        "Date": "2007-02-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 78.5199966430664
      },
      {
        "Date": "2007-02-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 74.12999725341797
      },
      {
        "Date": "2007-02-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 74.91999816894531
      },
      {
        "Date": "2007-03-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 75.08999633789062
      },
      {
        "Date": "2007-03-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 73.4000015258789
      },
      {
        "Date": "2007-03-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 71.63999938964844
      },
      {
        "Date": "2007-03-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 73.55000305175781
      },
      {
        "Date": "2007-03-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 73.88999938964844
      },
      {
        "Date": "2007-03-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 75.41000366210938
      },
      {"Date": "2007-03-09T00:00:00", "Bank": "MS", "Stock Price": 76},
      {
        "Date": "2007-03-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 76.05999755859375
      },
      {
        "Date": "2007-03-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 72.08000183105469
      },
      {
        "Date": "2007-03-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 73.80999755859375
      },
      {
        "Date": "2007-03-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 74.88999938964844
      },
      {
        "Date": "2007-03-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 74.41000366210938
      },
      {
        "Date": "2007-03-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 75.0199966430664
      },
      {
        "Date": "2007-03-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 76.11000061035156
      },
      {
        "Date": "2007-03-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.33000183105469
      },
      {
        "Date": "2007-03-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.12999725341797
      },
      {
        "Date": "2007-03-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.0999984741211
      },
      {
        "Date": "2007-03-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.37000274658203
      },
      {
        "Date": "2007-03-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 79.47000122070312
      },
      {
        "Date": "2007-03-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 78.33000183105469
      },
      {
        "Date": "2007-03-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 78.43000030517578
      },
      {
        "Date": "2007-03-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 78.76000213623047
      },
      {
        "Date": "2007-04-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 78.69000244140625
      },
      {
        "Date": "2007-04-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.18000030517578
      },
      {
        "Date": "2007-04-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 79.80999755859375
      },
      {
        "Date": "2007-04-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.30000305175781
      },
      {
        "Date": "2007-04-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.30000305175781
      },
      {
        "Date": "2007-04-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.27999877929688
      },
      {
        "Date": "2007-04-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 79.4000015258789
      },
      {
        "Date": "2007-04-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 80.06999969482422
      },
      {
        "Date": "2007-04-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 79.98999786376953
      },
      {
        "Date": "2007-04-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.06999969482422
      },
      {
        "Date": "2007-04-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.58999633789062
      },
      {
        "Date": "2007-04-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 81.81999969482422
      },
      {
        "Date": "2007-04-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.58999633789062
      },
      {
        "Date": "2007-04-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 82.91000366210938
      },
      {
        "Date": "2007-04-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.55999755859375
      },
      {
        "Date": "2007-04-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.51000213623047
      },
      {
        "Date": "2007-04-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.5199966430664
      },
      {
        "Date": "2007-04-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.37999725341797
      },
      {
        "Date": "2007-04-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.01000213623047
      },
      {
        "Date": "2007-04-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.01000213623047
      },
      {
        "Date": "2007-05-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.11000061035156
      },
      {
        "Date": "2007-05-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.36000061035156
      },
      {
        "Date": "2007-05-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.27999877929688
      },
      {
        "Date": "2007-05-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 86.56999969482422
      },
      {
        "Date": "2007-05-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.9800033569336
      },
      {
        "Date": "2007-05-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.6500015258789
      },
      {
        "Date": "2007-05-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 86.05000305175781
      },
      {
        "Date": "2007-05-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.37999725341797
      },
      {
        "Date": "2007-05-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.1500015258789
      },
      {
        "Date": "2007-05-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.9000015258789
      },
      {
        "Date": "2007-05-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.4800033569336
      },
      {
        "Date": "2007-05-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.08000183105469
      },
      {
        "Date": "2007-05-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.16999816894531
      },
      {
        "Date": "2007-05-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.05000305175781
      },
      {
        "Date": "2007-05-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.61000061035156
      },
      {
        "Date": "2007-05-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.62999725341797
      },
      {"Date": "2007-05-23T00:00:00", "Bank": "MS", "Stock Price": 85.75},
      {
        "Date": "2007-05-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.45999908447266
      },
      {
        "Date": "2007-05-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.26000213623047
      },
      {
        "Date": "2007-05-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.29000091552734
      },
      {
        "Date": "2007-05-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.81999969482422
      },
      {
        "Date": "2007-05-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.04000091552734
      },
      {
        "Date": "2007-06-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 86.06999969482422
      },
      {
        "Date": "2007-06-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.8499984741211
      },
      {
        "Date": "2007-06-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.6500015258789
      },
      {
        "Date": "2007-06-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.95999908447266
      },
      {
        "Date": "2007-06-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.7300033569336
      },
      {
        "Date": "2007-06-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 87.0999984741211
      },
      {
        "Date": "2007-06-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 88.54000091552734
      },
      {
        "Date": "2007-06-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 86.69999694824219
      },
      {
        "Date": "2007-06-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 89.16999816894531
      },
      {
        "Date": "2007-06-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 89.30000305175781
      },
      {
        "Date": "2007-06-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 88.4800033569336
      },
      {"Date": "2007-06-18T00:00:00", "Bank": "MS", "Stock Price": 88.5},
      {
        "Date": "2007-06-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 87.80000305175781
      },
      {
        "Date": "2007-06-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 87.31999969482422
      },
      {
        "Date": "2007-06-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 87.29000091552734
      },
      {
        "Date": "2007-06-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.5999984741211
      },
      {
        "Date": "2007-06-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.54000091552734
      },
      {
        "Date": "2007-06-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.11000061035156
      },
      {
        "Date": "2007-06-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 85.31999969482422
      },
      {
        "Date": "2007-06-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 84.87999725341797
      },
      {
        "Date": "2007-06-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 83.87999725341797
      },
      {
        "Date": "2007-07-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 71.33000183105469
      },
      {
        "Date": "2007-07-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 73.22000122070312
      },
      {
        "Date": "2007-07-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 72.94000244140625
      },
      {
        "Date": "2007-07-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 73.08999633789062
      },
      {
        "Date": "2007-07-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 72.66000366210938
      },
      {
        "Date": "2007-07-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 70.45999908447266
      },
      {
        "Date": "2007-07-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 70.6500015258789
      },
      {
        "Date": "2007-07-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 72.4000015258789
      },
      {
        "Date": "2007-07-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 73.26000213623047
      },
      {
        "Date": "2007-07-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 72.30000305175781
      },
      {
        "Date": "2007-07-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 72.8499984741211
      },
      {
        "Date": "2007-07-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 70.8499984741211
      },
      {
        "Date": "2007-07-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 69.87999725341797
      },
      {
        "Date": "2007-07-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.56999969482422
      },
      {
        "Date": "2007-07-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.70999908447266
      },
      {
        "Date": "2007-07-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 65.55000305175781
      },
      {
        "Date": "2007-07-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 65.86000061035156
      },
      {"Date": "2007-07-26T00:00:00", "Bank": "MS", "Stock Price": 64.5},
      {
        "Date": "2007-07-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.37000274658203
      },
      {
        "Date": "2007-07-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.61000061035156
      },
      {
        "Date": "2007-07-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.869998931884766
      },
      {
        "Date": "2007-08-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.37999725341797
      },
      {
        "Date": "2007-08-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.880001068115234
      },
      {
        "Date": "2007-08-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 60.619998931884766
      },
      {
        "Date": "2007-08-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.02999877929688
      },
      {
        "Date": "2007-08-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.33000183105469
      },
      {
        "Date": "2007-08-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 65.38999938964844
      },
      {
        "Date": "2007-08-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 61.810001373291016
      },
      {
        "Date": "2007-08-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 60.029998779296875
      },
      {
        "Date": "2007-08-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 59.63999938964844
      },
      {
        "Date": "2007-08-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 57.58000183105469
      },
      {
        "Date": "2007-08-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 56.630001068115234
      },
      {
        "Date": "2007-08-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 58.970001220703125
      },
      {
        "Date": "2007-08-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.22999954223633
      },
      {
        "Date": "2007-08-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.65999984741211
      },
      {
        "Date": "2007-08-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.88999938964844
      },
      {
        "Date": "2007-08-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.08999633789062
      },
      {
        "Date": "2007-08-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.30999755859375
      },
      {
        "Date": "2007-08-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.54000091552734
      },
      {
        "Date": "2007-08-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.72999954223633
      },
      {
        "Date": "2007-08-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 60.77000045776367
      },
      {
        "Date": "2007-08-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 61.209999084472656
      },
      {
        "Date": "2007-08-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 60.15999984741211
      },
      {
        "Date": "2007-08-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.369998931884766
      },
      {
        "Date": "2007-09-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.93000030517578
      },
      {
        "Date": "2007-09-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.560001373291016
      },
      {"Date": "2007-09-06T00:00:00", "Bank": "MS", "Stock Price": 62.5},
      {"Date": "2007-09-07T00:00:00", "Bank": "MS", "Stock Price": 62.5},
      {
        "Date": "2007-09-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.08000183105469
      },
      {
        "Date": "2007-09-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.540000915527344
      },
      {
        "Date": "2007-09-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.459999084472656
      },
      {
        "Date": "2007-09-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 66.79000091552734
      },
      {
        "Date": "2007-09-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 66.11000061035156
      },
      {
        "Date": "2007-09-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.91000366210938
      },
      {
        "Date": "2007-09-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 68.51000213623047
      },
      {
        "Date": "2007-09-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.02999877929688
      },
      {
        "Date": "2007-09-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.62999725341797
      },
      {
        "Date": "2007-09-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.44000244140625
      },
      {
        "Date": "2007-09-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.290000915527344
      },
      {
        "Date": "2007-09-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 61.369998931884766
      },
      {
        "Date": "2007-09-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.970001220703125
      },
      {
        "Date": "2007-09-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.55000305175781
      },
      {"Date": "2007-09-28T00:00:00", "Bank": "MS", "Stock Price": 63},
      {
        "Date": "2007-10-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.01000213623047
      },
      {
        "Date": "2007-10-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 66.0999984741211
      },
      {"Date": "2007-10-03T00:00:00", "Bank": "MS", "Stock Price": 67},
      {
        "Date": "2007-10-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.11000061035156
      },
      {
        "Date": "2007-10-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 68.9000015258789
      },
      {
        "Date": "2007-10-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.94000244140625
      },
      {
        "Date": "2007-10-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 69.08999633789062
      },
      {
        "Date": "2007-10-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.52999877929688
      },
      {
        "Date": "2007-10-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.05999755859375
      },
      {"Date": "2007-10-12T00:00:00", "Bank": "MS", "Stock Price": 67.25},
      {
        "Date": "2007-10-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 66.0999984741211
      },
      {
        "Date": "2007-10-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 65.30000305175781
      },
      {
        "Date": "2007-10-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 65.80999755859375
      },
      {
        "Date": "2007-10-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 65.4000015258789
      },
      {
        "Date": "2007-10-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 61.95000076293945
      },
      {
        "Date": "2007-10-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.59000015258789
      },
      {
        "Date": "2007-10-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 63.619998931884766
      },
      {
        "Date": "2007-10-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.88999938964844
      },
      {"Date": "2007-10-25T00:00:00", "Bank": "MS", "Stock Price": 62},
      {
        "Date": "2007-10-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 64.77999877929688
      },
      {
        "Date": "2007-10-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 66.2699966430664
      },
      {
        "Date": "2007-10-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 65.48999786376953
      },
      {
        "Date": "2007-10-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 67.26000213623047
      },
      {
        "Date": "2007-11-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 62.41999816894531
      },
      {
        "Date": "2007-11-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 58.900001525878906
      },
      {
        "Date": "2007-11-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 55.59000015258789
      },
      {
        "Date": "2007-11-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 54.5099983215332
      },
      {
        "Date": "2007-11-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 51.189998626708984
      },
      {
        "Date": "2007-11-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 53.68000030517578
      },
      {
        "Date": "2007-11-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 54.20000076293945
      },
      {
        "Date": "2007-11-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 53.77000045776367
      },
      {
        "Date": "2007-11-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 55.86000061035156
      },
      {
        "Date": "2007-11-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 55.61000061035156
      },
      {
        "Date": "2007-11-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 53.27000045776367
      },
      {
        "Date": "2007-11-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 52.900001525878906
      },
      {
        "Date": "2007-11-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 51.130001068115234
      },
      {
        "Date": "2007-11-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.43000030517578
      },
      {
        "Date": "2007-11-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.5099983215332
      },
      {
        "Date": "2007-11-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.88999938964844
      },
      {
        "Date": "2007-11-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.95000076293945
      },
      {
        "Date": "2007-11-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.79999923706055
      },
      {"Date": "2007-11-28T00:00:00", "Bank": "MS", "Stock Price": 53.5},
      {
        "Date": "2007-11-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 52.34000015258789
      },
      {
        "Date": "2007-11-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 52.720001220703125
      },
      {
        "Date": "2007-12-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 52.279998779296875
      },
      {
        "Date": "2007-12-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.0099983215332
      },
      {
        "Date": "2007-12-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.11000061035156
      },
      {
        "Date": "2007-12-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 51.58000183105469
      },
      {
        "Date": "2007-12-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 51.689998626708984
      },
      {
        "Date": "2007-12-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 54.369998931884766
      },
      {
        "Date": "2007-12-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.95000076293945
      },
      {
        "Date": "2007-12-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.369998931884766
      },
      {
        "Date": "2007-12-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.20000076293945
      },
      {
        "Date": "2007-12-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.29999923706055
      },
      {
        "Date": "2007-12-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.529998779296875
      },
      {
        "Date": "2007-12-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.06999969482422
      },
      {
        "Date": "2007-12-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.08000183105469
      },
      {
        "Date": "2007-12-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 51.369998931884766
      },
      {
        "Date": "2007-12-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 54.369998931884766
      },
      {
        "Date": "2007-12-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 54.970001220703125
      },
      {"Date": "2007-12-26T00:00:00", "Bank": "MS", "Stock Price": 55},
      {
        "Date": "2007-12-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 53.31999969482422
      },
      {
        "Date": "2007-12-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 53.220001220703125
      },
      {
        "Date": "2007-12-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 53.11000061035156
      },
      {
        "Date": "2008-01-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.95000076293945
      },
      {
        "Date": "2008-01-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.939998626708984
      },
      {
        "Date": "2008-01-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.29999923706055
      },
      {
        "Date": "2008-01-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.310001373291016
      },
      {
        "Date": "2008-01-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 46.400001525878906
      },
      {
        "Date": "2008-01-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.72999954223633
      },
      {
        "Date": "2008-01-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.40999984741211
      },
      {
        "Date": "2008-01-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.38999938964844
      },
      {
        "Date": "2008-01-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.900001525878906
      },
      {
        "Date": "2008-01-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.130001068115234
      },
      {
        "Date": "2008-01-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.38999938964844
      },
      {"Date": "2008-01-17T00:00:00", "Bank": "MS", "Stock Price": 45.25},
      {
        "Date": "2008-01-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.11000061035156
      },
      {
        "Date": "2008-01-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.529998779296875
      },
      {
        "Date": "2008-01-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 51.70000076293945
      },
      {
        "Date": "2008-01-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 51.22999954223633
      },
      {
        "Date": "2008-01-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.88999938964844
      },
      {
        "Date": "2008-01-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.59000015258789
      },
      {
        "Date": "2008-01-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.459999084472656
      },
      {
        "Date": "2008-01-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.630001068115234
      },
      {
        "Date": "2008-01-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.34000015258789
      },
      {"Date": "2008-02-01T00:00:00", "Bank": "MS", "Stock Price": 48.25},
      {
        "Date": "2008-02-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.029998779296875
      },
      {
        "Date": "2008-02-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.560001373291016
      },
      {
        "Date": "2008-02-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.95000076293945
      },
      {
        "Date": "2008-02-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.880001068115234
      },
      {
        "Date": "2008-02-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.189998626708984
      },
      {
        "Date": "2008-02-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.529998779296875
      },
      {
        "Date": "2008-02-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.709999084472656
      },
      {
        "Date": "2008-02-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.22999954223633
      },
      {
        "Date": "2008-02-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.619998931884766
      },
      {
        "Date": "2008-02-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.31999969482422
      },
      {
        "Date": "2008-02-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.4900016784668
      },
      {
        "Date": "2008-02-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.54999923706055
      },
      {
        "Date": "2008-02-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.16999816894531
      },
      {
        "Date": "2008-02-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.189998626708984
      },
      {
        "Date": "2008-02-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.279998779296875
      },
      {
        "Date": "2008-02-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.93000030517578
      },
      {
        "Date": "2008-02-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.880001068115234
      },
      {
        "Date": "2008-02-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.400001525878906
      },
      {
        "Date": "2008-02-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.119998931884766
      },
      {
        "Date": "2008-03-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.58000183105469
      },
      {
        "Date": "2008-03-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.349998474121094
      },
      {
        "Date": "2008-03-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.470001220703125
      },
      {
        "Date": "2008-03-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.66999816894531
      },
      {
        "Date": "2008-03-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.86000061035156
      },
      {
        "Date": "2008-03-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.29999923706055
      },
      {
        "Date": "2008-03-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.4900016784668
      },
      {
        "Date": "2008-03-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.0099983215332
      },
      {
        "Date": "2008-03-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.599998474121094
      },
      {
        "Date": "2008-03-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.54999923706055
      },
      {
        "Date": "2008-03-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 36.380001068115234
      },
      {
        "Date": "2008-03-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.86000061035156
      },
      {
        "Date": "2008-03-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.45000076293945
      },
      {
        "Date": "2008-03-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.66999816894531
      },
      {"Date": "2008-03-24T00:00:00", "Bank": "MS", "Stock Price": 48.75},
      {
        "Date": "2008-03-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.45000076293945
      },
      {
        "Date": "2008-03-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.790000915527344
      },
      {
        "Date": "2008-03-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.689998626708984
      },
      {
        "Date": "2008-03-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.7400016784668
      },
      {
        "Date": "2008-03-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.70000076293945
      },
      {
        "Date": "2008-04-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.849998474121094
      },
      {
        "Date": "2008-04-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.09000015258789
      },
      {
        "Date": "2008-04-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.880001068115234
      },
      {
        "Date": "2008-04-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.599998474121094
      },
      {
        "Date": "2008-04-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.09000015258789
      },
      {
        "Date": "2008-04-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.619998931884766
      },
      {
        "Date": "2008-04-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 46.099998474121094
      },
      {
        "Date": "2008-04-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.439998626708984
      },
      {
        "Date": "2008-04-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.630001068115234
      },
      {
        "Date": "2008-04-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.970001220703125
      },
      {
        "Date": "2008-04-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.52000045776367
      },
      {
        "Date": "2008-04-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.41999816894531
      },
      {
        "Date": "2008-04-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 46.41999816894531
      },
      {
        "Date": "2008-04-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.77000045776367
      },
      {
        "Date": "2008-04-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.20000076293945
      },
      {
        "Date": "2008-04-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.189998626708984
      },
      {
        "Date": "2008-04-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.380001068115234
      },
      {
        "Date": "2008-04-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.38999938964844
      },
      {
        "Date": "2008-04-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.650001525878906
      },
      {
        "Date": "2008-04-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.90999984741211
      },
      {
        "Date": "2008-04-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.959999084472656
      },
      {
        "Date": "2008-04-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.599998474121094
      },
      {
        "Date": "2008-05-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.33000183105469
      },
      {
        "Date": "2008-05-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 50.310001373291016
      },
      {
        "Date": "2008-05-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 48.720001220703125
      },
      {
        "Date": "2008-05-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 49.04999923706055
      },
      {
        "Date": "2008-05-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.209999084472656
      },
      {
        "Date": "2008-05-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 46.47999954223633
      },
      {
        "Date": "2008-05-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.959999084472656
      },
      {
        "Date": "2008-05-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.650001525878906
      },
      {
        "Date": "2008-05-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 46.61000061035156
      },
      {
        "Date": "2008-05-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 46.959999084472656
      },
      {
        "Date": "2008-05-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.709999084472656
      },
      {
        "Date": "2008-05-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 47.209999084472656
      },
      {
        "Date": "2008-05-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 46.20000076293945
      },
      {
        "Date": "2008-05-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.79999923706055
      },
      {
        "Date": "2008-05-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.88999938964844
      },
      {
        "Date": "2008-05-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.95000076293945
      },
      {
        "Date": "2008-05-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.83000183105469
      },
      {
        "Date": "2008-05-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.2400016784668
      },
      {
        "Date": "2008-05-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.77000045776367
      },
      {
        "Date": "2008-05-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.779998779296875
      },
      {
        "Date": "2008-05-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.22999954223633
      },
      {
        "Date": "2008-06-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.099998474121094
      },
      {
        "Date": "2008-06-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.650001525878906
      },
      {
        "Date": "2008-06-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.36000061035156
      },
      {
        "Date": "2008-06-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 44.59000015258789
      },
      {
        "Date": "2008-06-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.810001373291016
      },
      {
        "Date": "2008-06-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.38999938964844
      },
      {
        "Date": "2008-06-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.22999954223633
      },
      {
        "Date": "2008-06-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 37.130001068115234
      },
      {
        "Date": "2008-06-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.380001068115234
      },
      {
        "Date": "2008-06-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.040000915527344
      },
      {
        "Date": "2008-06-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.290000915527344
      },
      {
        "Date": "2008-06-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.59000015258789
      },
      {
        "Date": "2008-06-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.689998626708984
      },
      {
        "Date": "2008-06-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.189998626708984
      },
      {
        "Date": "2008-06-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.68000030517578
      },
      {
        "Date": "2008-06-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 37.459999084472656
      },
      {
        "Date": "2008-06-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.43000030517578
      },
      {
        "Date": "2008-06-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.18000030517578
      },
      {
        "Date": "2008-06-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 36.83000183105469
      },
      {
        "Date": "2008-06-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 36.709999084472656
      },
      {
        "Date": "2008-06-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 36.06999969482422
      },
      {
        "Date": "2008-07-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 36.599998474121094
      },
      {
        "Date": "2008-07-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 35.869998931884766
      },
      {
        "Date": "2008-07-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 35.90999984741211
      },
      {
        "Date": "2008-07-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 35.06999969482422
      },
      {
        "Date": "2008-07-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 36.4900016784668
      },
      {
        "Date": "2008-07-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.9900016784668
      },
      {
        "Date": "2008-07-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.5099983215332
      },
      {
        "Date": "2008-07-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.439998626708984
      },
      {"Date": "2008-07-14T00:00:00", "Bank": "MS", "Stock Price": 31.75},
      {"Date": "2008-07-15T00:00:00", "Bank": "MS", "Stock Price": 31},
      {
        "Date": "2008-07-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 35.04999923706055
      },
      {
        "Date": "2008-07-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.31999969482422
      },
      {
        "Date": "2008-07-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.56999969482422
      },
      {
        "Date": "2008-07-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 36.459999084472656
      },
      {
        "Date": "2008-07-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.66999816894531
      },
      {
        "Date": "2008-07-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.11000061035156
      },
      {
        "Date": "2008-07-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 37.2400016784668
      },
      {"Date": "2008-07-25T00:00:00", "Bank": "MS", "Stock Price": 36.75},
      {
        "Date": "2008-07-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 34.959999084472656
      },
      {"Date": "2008-07-29T00:00:00", "Bank": "MS", "Stock Price": 36.5},
      {
        "Date": "2008-07-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.599998474121094
      },
      {
        "Date": "2008-07-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.47999954223633
      },
      {
        "Date": "2008-08-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.11000061035156
      },
      {
        "Date": "2008-08-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.47999954223633
      },
      {
        "Date": "2008-08-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.20000076293945
      },
      {
        "Date": "2008-08-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.18000030517578
      },
      {
        "Date": "2008-08-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.65999984741211
      },
      {
        "Date": "2008-08-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.040000915527344
      },
      {
        "Date": "2008-08-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 45.38999938964844
      },
      {"Date": "2008-08-12T00:00:00", "Bank": "MS", "Stock Price": 42.5},
      {
        "Date": "2008-08-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.150001525878906
      },
      {
        "Date": "2008-08-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.63999938964844
      },
      {
        "Date": "2008-08-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.880001068115234
      },
      {
        "Date": "2008-08-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.59000015258789
      },
      {
        "Date": "2008-08-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.08000183105469
      },
      {
        "Date": "2008-08-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 37.400001525878906
      },
      {
        "Date": "2008-08-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 37.060001373291016
      },
      {
        "Date": "2008-08-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.88999938964844
      },
      {
        "Date": "2008-08-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.220001220703125
      },
      {
        "Date": "2008-08-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.58000183105469
      },
      {
        "Date": "2008-08-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 39.04999923706055
      },
      {
        "Date": "2008-08-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.599998474121094
      },
      {
        "Date": "2008-08-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.83000183105469
      },
      {
        "Date": "2008-09-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.29999923706055
      },
      {
        "Date": "2008-09-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 42.16999816894531
      },
      {
        "Date": "2008-09-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.34000015258789
      },
      {
        "Date": "2008-09-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 41.36000061035156
      },
      {
        "Date": "2008-09-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 43.27000045776367
      },
      {
        "Date": "2008-09-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 40.400001525878906
      },
      {
        "Date": "2008-09-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.91999816894531
      },
      {
        "Date": "2008-09-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 38.709999084472656
      },
      {
        "Date": "2008-09-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 37.22999954223633
      },
      {
        "Date": "2008-09-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.189998626708984
      },
      {
        "Date": "2008-09-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.700000762939453
      },
      {"Date": "2008-09-17T00:00:00", "Bank": "MS", "Stock Price": 21.75},
      {
        "Date": "2008-09-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.549999237060547
      },
      {
        "Date": "2008-09-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.209999084472656
      },
      {
        "Date": "2008-09-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.09000015258789
      },
      {"Date": "2008-09-23T00:00:00", "Bank": "MS", "Stock Price": 28},
      {
        "Date": "2008-09-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.790000915527344
      },
      {
        "Date": "2008-09-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.100000381469727
      },
      {"Date": "2008-09-26T00:00:00", "Bank": "MS", "Stock Price": 24.75},
      {
        "Date": "2008-09-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.989999771118164
      },
      {"Date": "2008-09-30T00:00:00", "Bank": "MS", "Stock Price": 23},
      {
        "Date": "2008-10-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.420000076293945
      },
      {
        "Date": "2008-10-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.209999084472656
      },
      {
        "Date": "2008-10-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.920000076293945
      },
      {"Date": "2008-10-06T00:00:00", "Bank": "MS", "Stock Price": 23.5},
      {
        "Date": "2008-10-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.649999618530273
      },
      {
        "Date": "2008-10-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.799999237060547
      },
      {
        "Date": "2008-10-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 12.449999809265137
      },
      {
        "Date": "2008-10-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 9.680000305175781
      },
      {
        "Date": "2008-10-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.100000381469727
      },
      {
        "Date": "2008-10-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.940000534057617
      },
      {
        "Date": "2008-10-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.1299991607666
      },
      {
        "Date": "2008-10-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.690000534057617
      },
      {
        "Date": "2008-10-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.239999771118164
      },
      {
        "Date": "2008-10-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.770000457763672
      },
      {
        "Date": "2008-10-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.200000762939453
      },
      {
        "Date": "2008-10-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.329999923706055
      },
      {
        "Date": "2008-10-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.079999923706055
      },
      {
        "Date": "2008-10-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.520000457763672
      },
      {
        "Date": "2008-10-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.729999542236328
      },
      {
        "Date": "2008-10-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 15.199999809265137
      },
      {
        "Date": "2008-10-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.760000228881836
      },
      {
        "Date": "2008-10-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.09000015258789
      },
      {
        "Date": "2008-10-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.469999313354492
      },
      {"Date": "2008-11-03T00:00:00", "Bank": "MS", "Stock Price": 18},
      {
        "Date": "2008-11-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.899999618530273
      },
      {
        "Date": "2008-11-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.059999465942383
      },
      {
        "Date": "2008-11-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 15.390000343322754
      },
      {
        "Date": "2008-11-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 15.979999542236328
      },
      {
        "Date": "2008-11-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.579999923706055
      },
      {
        "Date": "2008-11-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.079999923706055
      },
      {
        "Date": "2008-11-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 11.9399995803833
      },
      {
        "Date": "2008-11-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.210000038146973
      },
      {
        "Date": "2008-11-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 12.029999732971191
      },
      {
        "Date": "2008-11-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 11.220000267028809
      },
      {
        "Date": "2008-11-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 12.029999732971191
      },
      {"Date": "2008-11-19T00:00:00", "Bank": "MS", "Stock Price": 10.25},
      {
        "Date": "2008-11-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 9.199999809265137
      },
      {
        "Date": "2008-11-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 10.050000190734863
      },
      {
        "Date": "2008-11-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.380000114440918
      },
      {
        "Date": "2008-11-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.270000457763672
      },
      {"Date": "2008-11-26T00:00:00", "Bank": "MS", "Stock Price": 14.5},
      {"Date": "2008-11-28T00:00:00", "Bank": "MS", "Stock Price": 14.75},
      {
        "Date": "2008-12-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 11.350000381469727
      },
      {
        "Date": "2008-12-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 12.039999961853027
      },
      {
        "Date": "2008-12-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.850000381469727
      },
      {
        "Date": "2008-12-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.9399995803833
      },
      {
        "Date": "2008-12-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 15.720000267028809
      },
      {
        "Date": "2008-12-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.299999237060547
      },
      {
        "Date": "2008-12-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.970000267028809
      },
      {
        "Date": "2008-12-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.600000381469727
      },
      {
        "Date": "2008-12-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.739999771118164
      },
      {
        "Date": "2008-12-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.850000381469727
      },
      {
        "Date": "2008-12-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.640000343322754
      },
      {
        "Date": "2008-12-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.1299991607666
      },
      {"Date": "2008-12-17T00:00:00", "Bank": "MS", "Stock Price": 16.5},
      {
        "Date": "2008-12-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.229999542236328
      },
      {
        "Date": "2008-12-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 15.449999809265137
      },
      {
        "Date": "2008-12-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.579999923706055
      },
      {
        "Date": "2008-12-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.4399995803833
      },
      {"Date": "2008-12-24T00:00:00", "Bank": "MS", "Stock Price": 14.5},
      {
        "Date": "2008-12-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.649999618530273
      },
      {
        "Date": "2008-12-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 14.899999618530273
      },
      {
        "Date": "2008-12-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 15.1899995803833
      },
      {
        "Date": "2008-12-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.040000915527344
      },
      {
        "Date": "2009-01-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.989999771118164
      },
      {
        "Date": "2009-01-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.6200008392334
      },
      {
        "Date": "2009-01-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.579999923706055
      },
      {
        "Date": "2009-01-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.100000381469727
      },
      {
        "Date": "2009-01-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.81999969482422
      },
      {
        "Date": "2009-01-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.059999465942383
      },
      {
        "Date": "2009-01-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.790000915527344
      },
      {
        "Date": "2009-01-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.860000610351562
      },
      {
        "Date": "2009-01-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.190000534057617
      },
      {
        "Date": "2009-01-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.260000228881836
      },
      {
        "Date": "2009-01-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 15.59000015258789
      },
      {
        "Date": "2009-01-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 13.100000381469727
      },
      {
        "Date": "2009-01-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.860000610351562
      },
      {
        "Date": "2009-01-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.579999923706055
      },
      {
        "Date": "2009-01-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.709999084472656
      },
      {
        "Date": "2009-01-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.079999923706055
      },
      {
        "Date": "2009-01-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.790000915527344
      },
      {"Date": "2009-01-28T00:00:00", "Bank": "MS", "Stock Price": 23},
      {
        "Date": "2009-01-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.3799991607666
      },
      {
        "Date": "2009-01-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.229999542236328
      },
      {
        "Date": "2009-02-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.799999237060547
      },
      {
        "Date": "2009-02-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.940000534057617
      },
      {
        "Date": "2009-02-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.010000228881836
      },
      {
        "Date": "2009-02-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.190000534057617
      },
      {
        "Date": "2009-02-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.8700008392334
      },
      {
        "Date": "2009-02-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.610000610351562
      },
      {
        "Date": "2009-02-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.790000915527344
      },
      {
        "Date": "2009-02-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.90999984741211
      },
      {
        "Date": "2009-02-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.989999771118164
      },
      {
        "Date": "2009-02-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.93000030517578
      },
      {
        "Date": "2009-02-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.760000228881836
      },
      {
        "Date": "2009-02-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.18000030517578
      },
      {
        "Date": "2009-02-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.93000030517578
      },
      {
        "Date": "2009-02-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.43000030517578
      },
      {
        "Date": "2009-02-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.81999969482422
      },
      {
        "Date": "2009-02-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.06999969482422
      },
      {
        "Date": "2009-02-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.760000228881836
      },
      {
        "Date": "2009-02-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.329999923706055
      },
      {
        "Date": "2009-02-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.540000915527344
      },
      {
        "Date": "2009-03-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.950000762939453
      },
      {
        "Date": "2009-03-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 18.18000030517578
      },
      {
        "Date": "2009-03-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 19.399999618530273
      },
      {
        "Date": "2009-03-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.979999542236328
      },
      {
        "Date": "2009-03-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 17.18000030517578
      },
      {
        "Date": "2009-03-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 16.479999542236328
      },
      {
        "Date": "2009-03-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.84000015258789
      },
      {
        "Date": "2009-03-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.510000228881836
      },
      {
        "Date": "2009-03-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.18000030517578
      },
      {
        "Date": "2009-03-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.43000030517578
      },
      {
        "Date": "2009-03-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.040000915527344
      },
      {
        "Date": "2009-03-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.809999465942383
      },
      {
        "Date": "2009-03-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.190000534057617
      },
      {
        "Date": "2009-03-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.040000915527344
      },
      {
        "Date": "2009-03-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 20.239999771118164
      },
      {
        "Date": "2009-03-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.43000030517578
      },
      {
        "Date": "2009-03-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.1200008392334
      },
      {
        "Date": "2009-03-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.90999984741211
      },
      {
        "Date": "2009-03-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.649999618530273
      },
      {
        "Date": "2009-03-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.350000381469727
      },
      {
        "Date": "2009-03-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.1299991607666
      },
      {
        "Date": "2009-03-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.770000457763672
      },
      {
        "Date": "2009-04-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.729999542236328
      },
      {
        "Date": "2009-04-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.110000610351562
      },
      {
        "Date": "2009-04-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.059999465942383
      },
      {
        "Date": "2009-04-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.309999465942383
      },
      {
        "Date": "2009-04-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.31999969482422
      },
      {
        "Date": "2009-04-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.690000534057617
      },
      {
        "Date": "2009-04-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.350000381469727
      },
      {
        "Date": "2009-04-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.889999389648438
      },
      {
        "Date": "2009-04-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.670000076293945
      },
      {
        "Date": "2009-04-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.450000762939453
      },
      {
        "Date": "2009-04-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.969999313354492
      },
      {"Date": "2009-04-17T00:00:00", "Bank": "MS", "Stock Price": 25},
      {
        "Date": "2009-04-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.520000457763672
      },
      {
        "Date": "2009-04-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.649999618530273
      },
      {
        "Date": "2009-04-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.440000534057617
      },
      {
        "Date": "2009-04-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.959999084472656
      },
      {
        "Date": "2009-04-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.959999084472656
      },
      {
        "Date": "2009-04-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.260000228881836
      },
      {
        "Date": "2009-04-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 21.079999923706055
      },
      {
        "Date": "2009-04-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.06999969482422
      },
      {
        "Date": "2009-04-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.639999389648438
      },
      {
        "Date": "2009-05-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.81999969482422
      },
      {
        "Date": "2009-05-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.020000457763672
      },
      {
        "Date": "2009-05-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.209999084472656
      },
      {
        "Date": "2009-05-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.510000228881836
      },
      {
        "Date": "2009-05-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.139999389648438
      },
      {
        "Date": "2009-05-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.200000762939453
      },
      {
        "Date": "2009-05-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.06999969482422
      },
      {
        "Date": "2009-05-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.420000076293945
      },
      {
        "Date": "2009-05-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.100000381469727
      },
      {
        "Date": "2009-05-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.56999969482422
      },
      {
        "Date": "2009-05-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.1299991607666
      },
      {
        "Date": "2009-05-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.280000686645508
      },
      {
        "Date": "2009-05-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.90999984741211
      },
      {"Date": "2009-05-20T00:00:00", "Bank": "MS", "Stock Price": 28},
      {
        "Date": "2009-05-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.09000015258789
      },
      {
        "Date": "2009-05-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.229999542236328
      },
      {
        "Date": "2009-05-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.020000457763672
      },
      {
        "Date": "2009-05-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.610000610351562
      },
      {
        "Date": "2009-05-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.43000030517578
      },
      {
        "Date": "2009-05-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.31999969482422
      },
      {
        "Date": "2009-06-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.889999389648438
      },
      {
        "Date": "2009-06-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.09000015258789
      },
      {
        "Date": "2009-06-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.719999313354492
      },
      {
        "Date": "2009-06-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.200000762939453
      },
      {
        "Date": "2009-06-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.969999313354492
      },
      {
        "Date": "2009-06-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.389999389648438
      },
      {
        "Date": "2009-06-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.979999542236328
      },
      {
        "Date": "2009-06-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.260000228881836
      },
      {
        "Date": "2009-06-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.489999771118164
      },
      {
        "Date": "2009-06-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.700000762939453
      },
      {
        "Date": "2009-06-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.399999618530273
      },
      {
        "Date": "2009-06-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.100000381469727
      },
      {
        "Date": "2009-06-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.479999542236328
      },
      {
        "Date": "2009-06-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.030000686645508
      },
      {
        "Date": "2009-06-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.270000457763672
      },
      {
        "Date": "2009-06-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.6299991607666
      },
      {
        "Date": "2009-06-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.700000762939453
      },
      {
        "Date": "2009-06-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.649999618530273
      },
      {
        "Date": "2009-06-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.8700008392334
      },
      {
        "Date": "2009-06-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.6200008392334
      },
      {
        "Date": "2009-06-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.100000381469727
      },
      {
        "Date": "2009-06-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.510000228881836
      },
      {
        "Date": "2009-07-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.360000610351562
      },
      {
        "Date": "2009-07-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.989999771118164
      },
      {
        "Date": "2009-07-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.850000381469727
      },
      {
        "Date": "2009-07-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.149999618530273
      },
      {"Date": "2009-07-08T00:00:00", "Bank": "MS", "Stock Price": 25.5},
      {
        "Date": "2009-07-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.8799991607666
      },
      {
        "Date": "2009-07-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.940000534057617
      },
      {
        "Date": "2009-07-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.90999984741211
      },
      {
        "Date": "2009-07-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.8799991607666
      },
      {
        "Date": "2009-07-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.799999237060547
      },
      {
        "Date": "2009-07-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.559999465942383
      },
      {
        "Date": "2009-07-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.989999771118164
      },
      {
        "Date": "2009-07-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.34000015258789
      },
      {
        "Date": "2009-07-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.559999465942383
      },
      {
        "Date": "2009-07-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.540000915527344
      },
      {
        "Date": "2009-07-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.540000915527344
      },
      {"Date": "2009-07-24T00:00:00", "Bank": "MS", "Stock Price": 28.25},
      {
        "Date": "2009-07-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.049999237060547
      },
      {
        "Date": "2009-07-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.43000030517578
      },
      {
        "Date": "2009-07-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.15999984741211
      },
      {
        "Date": "2009-07-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.360000610351562
      },
      {"Date": "2009-07-31T00:00:00", "Bank": "MS", "Stock Price": 28.5},
      {
        "Date": "2009-08-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.309999465942383
      },
      {
        "Date": "2009-08-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.06999969482422
      },
      {
        "Date": "2009-08-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.049999237060547
      },
      {
        "Date": "2009-08-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.549999237060547
      },
      {
        "Date": "2009-08-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.219999313354492
      },
      {
        "Date": "2009-08-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.829999923706055
      },
      {
        "Date": "2009-08-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.889999389648438
      },
      {
        "Date": "2009-08-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.979999542236328
      },
      {
        "Date": "2009-08-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.8799991607666
      },
      {
        "Date": "2009-08-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.790000915527344
      },
      {
        "Date": "2009-08-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.540000915527344
      },
      {
        "Date": "2009-08-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.780000686645508
      },
      {
        "Date": "2009-08-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.829999923706055
      },
      {
        "Date": "2009-08-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.360000610351562
      },
      {
        "Date": "2009-08-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.690000534057617
      },
      {
        "Date": "2009-08-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.649999618530273
      },
      {
        "Date": "2009-08-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.190000534057617
      },
      {
        "Date": "2009-08-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.530000686645508
      },
      {
        "Date": "2009-08-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.84000015258789
      },
      {
        "Date": "2009-08-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.510000228881836
      },
      {
        "Date": "2009-08-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.959999084472656
      },
      {
        "Date": "2009-09-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.450000762939453
      },
      {
        "Date": "2009-09-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.09000015258789
      },
      {
        "Date": "2009-09-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.649999618530273
      },
      {
        "Date": "2009-09-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.649999618530273
      },
      {
        "Date": "2009-09-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.799999237060547
      },
      {
        "Date": "2009-09-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.549999237060547
      },
      {
        "Date": "2009-09-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.639999389648438
      },
      {
        "Date": "2009-09-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.81999969482422
      },
      {"Date": "2009-09-14T00:00:00", "Bank": "MS", "Stock Price": 28.75},
      {
        "Date": "2009-09-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.739999771118164
      },
      {
        "Date": "2009-09-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.149999618530273
      },
      {
        "Date": "2009-09-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.049999237060547
      },
      {
        "Date": "2009-09-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.3799991607666
      },
      {
        "Date": "2009-09-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.610000610351562
      },
      {
        "Date": "2009-09-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.97999954223633
      },
      {
        "Date": "2009-09-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.029998779296875
      },
      {
        "Date": "2009-09-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.729999542236328
      },
      {
        "Date": "2009-09-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.549999237060547
      },
      {"Date": "2009-09-28T00:00:00", "Bank": "MS", "Stock Price": 31.25},
      {
        "Date": "2009-09-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.09000015258789
      },
      {
        "Date": "2009-09-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.8799991607666
      },
      {
        "Date": "2009-10-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.8700008392334
      },
      {
        "Date": "2009-10-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.459999084472656
      },
      {
        "Date": "2009-10-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.84000015258789
      },
      {
        "Date": "2009-10-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.790000915527344
      },
      {
        "Date": "2009-10-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.15999984741211
      },
      {
        "Date": "2009-10-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.940000534057617
      },
      {
        "Date": "2009-10-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.09000015258789
      },
      {
        "Date": "2009-10-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.760000228881836
      },
      {
        "Date": "2009-10-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.139999389648438
      },
      {
        "Date": "2009-10-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.83000183105469
      },
      {
        "Date": "2009-10-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.709999084472656
      },
      {
        "Date": "2009-10-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.9900016784668
      },
      {
        "Date": "2009-10-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.11000061035156
      },
      {
        "Date": "2009-10-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.52000045776367
      },
      {
        "Date": "2009-10-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 34.08000183105469
      },
      {
        "Date": "2009-10-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 35.7400016784668
      },
      {"Date": "2009-10-23T00:00:00", "Bank": "MS", "Stock Price": 35},
      {
        "Date": "2009-10-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 34.79999923706055
      },
      {
        "Date": "2009-10-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 34.11000061035156
      },
      {
        "Date": "2009-10-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.310001373291016
      },
      {
        "Date": "2009-10-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.66999816894531
      },
      {
        "Date": "2009-10-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.119998931884766
      },
      {
        "Date": "2009-11-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.979999542236328
      },
      {
        "Date": "2009-11-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.13999938964844
      },
      {
        "Date": "2009-11-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.479999542236328
      },
      {
        "Date": "2009-11-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.41999816894531
      },
      {
        "Date": "2009-11-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.599998474121094
      },
      {
        "Date": "2009-11-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.95000076293945
      },
      {
        "Date": "2009-11-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.70000076293945
      },
      {"Date": "2009-11-11T00:00:00", "Bank": "MS", "Stock Price": 33.75},
      {
        "Date": "2009-11-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.0099983215332
      },
      {
        "Date": "2009-11-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.09000015258789
      },
      {
        "Date": "2009-11-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 34.22999954223633
      },
      {
        "Date": "2009-11-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.470001220703125
      },
      {
        "Date": "2009-11-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 33.33000183105469
      },
      {
        "Date": "2009-11-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.310001373291016
      },
      {
        "Date": "2009-11-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.099998474121094
      },
      {
        "Date": "2009-11-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.619998931884766
      },
      {
        "Date": "2009-11-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.119998931884766
      },
      {
        "Date": "2009-11-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.420000076293945
      },
      {
        "Date": "2009-11-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.510000228881836
      },
      {
        "Date": "2009-11-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.579999923706055
      },
      {
        "Date": "2009-12-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.520000457763672
      },
      {
        "Date": "2009-12-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.600000381469727
      },
      {
        "Date": "2009-12-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.200000762939453
      },
      {
        "Date": "2009-12-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.969999313354492
      },
      {
        "Date": "2009-12-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.3799991607666
      },
      {
        "Date": "2009-12-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.149999618530273
      },
      {
        "Date": "2009-12-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.350000381469727
      },
      {
        "Date": "2009-12-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.229999542236328
      },
      {
        "Date": "2009-12-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.780000686645508
      },
      {
        "Date": "2009-12-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.170000076293945
      },
      {
        "Date": "2009-12-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.850000381469727
      },
      {
        "Date": "2009-12-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.34000015258789
      },
      {
        "Date": "2009-12-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.1200008392334
      },
      {
        "Date": "2009-12-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.209999084472656
      },
      {
        "Date": "2009-12-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.65999984741211
      },
      {
        "Date": "2009-12-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.600000381469727
      },
      {
        "Date": "2009-12-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.40999984741211
      },
      {
        "Date": "2009-12-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.600000381469727
      },
      {
        "Date": "2009-12-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.290000915527344
      },
      {
        "Date": "2009-12-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.43000030517578
      },
      {
        "Date": "2009-12-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.489999771118164
      },
      {
        "Date": "2009-12-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.600000381469727
      },
      {
        "Date": "2010-01-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.90999984741211
      },
      {
        "Date": "2010-01-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.040000915527344
      },
      {
        "Date": "2010-01-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.45000076293945
      },
      {
        "Date": "2010-01-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.91999816894531
      },
      {"Date": "2010-01-08T00:00:00", "Bank": "MS", "Stock Price": 32.25},
      {
        "Date": "2010-01-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 32.040000915527344
      },
      {
        "Date": "2010-01-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.1299991607666
      },
      {
        "Date": "2010-01-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.260000228881836
      },
      {
        "Date": "2010-01-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.200000762939453
      },
      {
        "Date": "2010-01-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.3799991607666
      },
      {
        "Date": "2010-01-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.15999984741211
      },
      {
        "Date": "2010-01-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.6299991607666
      },
      {
        "Date": "2010-01-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.34000015258789
      },
      {
        "Date": "2010-01-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.799999237060547
      },
      {
        "Date": "2010-01-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.739999771118164
      },
      {
        "Date": "2010-01-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.329999923706055
      },
      {
        "Date": "2010-01-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.950000762939453
      },
      {
        "Date": "2010-01-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.489999771118164
      },
      {
        "Date": "2010-01-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.780000686645508
      },
      {
        "Date": "2010-02-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.559999465942383
      },
      {
        "Date": "2010-02-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.059999465942383
      },
      {
        "Date": "2010-02-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.889999389648438
      },
      {
        "Date": "2010-02-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.6299991607666
      },
      {
        "Date": "2010-02-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.260000228881836
      },
      {
        "Date": "2010-02-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.600000381469727
      },
      {
        "Date": "2010-02-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.1299991607666
      },
      {
        "Date": "2010-02-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.510000228881836
      },
      {
        "Date": "2010-02-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.1200008392334
      },
      {
        "Date": "2010-02-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.15999984741211
      },
      {
        "Date": "2010-02-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.81999969482422
      },
      {
        "Date": "2010-02-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.389999389648438
      },
      {
        "Date": "2010-02-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.260000228881836
      },
      {
        "Date": "2010-02-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.40999984741211
      },
      {
        "Date": "2010-02-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.709999084472656
      },
      {
        "Date": "2010-02-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.149999618530273
      },
      {
        "Date": "2010-02-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.829999923706055
      },
      {
        "Date": "2010-02-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.739999771118164
      },
      {
        "Date": "2010-02-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.18000030517578
      },
      {
        "Date": "2010-03-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.190000534057617
      },
      {
        "Date": "2010-03-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.700000762939453
      },
      {
        "Date": "2010-03-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.31999969482422
      },
      {
        "Date": "2010-03-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.200000762939453
      },
      {
        "Date": "2010-03-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.40999984741211
      },
      {
        "Date": "2010-03-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.579999923706055
      },
      {
        "Date": "2010-03-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.049999237060547
      },
      {
        "Date": "2010-03-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.969999313354492
      },
      {
        "Date": "2010-03-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.020000457763672
      },
      {
        "Date": "2010-03-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.90999984741211
      },
      {
        "Date": "2010-03-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.639999389648438
      },
      {
        "Date": "2010-03-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.309999465942383
      },
      {
        "Date": "2010-03-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.280000686645508
      },
      {
        "Date": "2010-03-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.079999923706055
      },
      {
        "Date": "2010-03-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.6299991607666
      },
      {
        "Date": "2010-03-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.600000381469727
      },
      {
        "Date": "2010-03-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.530000686645508
      },
      {
        "Date": "2010-03-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.3700008392334
      },
      {
        "Date": "2010-03-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.90999984741211
      },
      {
        "Date": "2010-03-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.850000381469727
      },
      {
        "Date": "2010-03-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.43000030517578
      },
      {
        "Date": "2010-03-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.209999084472656
      },
      {
        "Date": "2010-03-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.290000915527344
      },
      {
        "Date": "2010-04-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.200000762939453
      },
      {
        "Date": "2010-04-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.290000915527344
      },
      {
        "Date": "2010-04-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.360000610351562
      },
      {
        "Date": "2010-04-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.020000457763672
      },
      {
        "Date": "2010-04-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.8799991607666
      },
      {
        "Date": "2010-04-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.979999542236328
      },
      {
        "Date": "2010-04-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.93000030517578
      },
      {
        "Date": "2010-04-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.479999542236328
      },
      {
        "Date": "2010-04-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.139999389648438
      },
      {
        "Date": "2010-04-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.8799991607666
      },
      {
        "Date": "2010-04-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.15999984741211
      },
      {
        "Date": "2010-04-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.559999465942383
      },
      {
        "Date": "2010-04-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.450000762939453
      },
      {
        "Date": "2010-04-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.68000030517578
      },
      {
        "Date": "2010-04-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.899999618530273
      },
      {
        "Date": "2010-04-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.940000534057617
      },
      {
        "Date": "2010-04-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.940000534057617
      },
      {
        "Date": "2010-04-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.93000030517578
      },
      {
        "Date": "2010-04-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.329999923706055
      },
      {
        "Date": "2010-04-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 31.309999465942383
      },
      {
        "Date": "2010-04-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.219999313354492
      },
      {
        "Date": "2010-05-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 30.43000030517578
      },
      {
        "Date": "2010-05-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.489999771118164
      },
      {
        "Date": "2010-05-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 29.290000915527344
      },
      {
        "Date": "2010-05-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.639999389648438
      },
      {"Date": "2010-05-07T00:00:00", "Bank": "MS", "Stock Price": 27.75},
      {
        "Date": "2010-05-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.860000610351562
      },
      {
        "Date": "2010-05-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 28.3799991607666
      },
      {
        "Date": "2010-05-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.799999237060547
      },
      {
        "Date": "2010-05-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.6200008392334
      },
      {
        "Date": "2010-05-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.079999923706055
      },
      {
        "Date": "2010-05-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.110000610351562
      },
      {
        "Date": "2010-05-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.729999542236328
      },
      {
        "Date": "2010-05-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.040000915527344
      },
      {
        "Date": "2010-05-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.639999389648438
      },
      {
        "Date": "2010-05-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.110000610351562
      },
      {"Date": "2010-05-24T00:00:00", "Bank": "MS", "Stock Price": 25.75},
      {
        "Date": "2010-05-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.110000610351562
      },
      {
        "Date": "2010-05-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.530000686645508
      },
      {
        "Date": "2010-05-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.65999984741211
      },
      {
        "Date": "2010-05-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.110000610351562
      },
      {
        "Date": "2010-06-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.1299991607666
      },
      {
        "Date": "2010-06-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.18000030517578
      },
      {
        "Date": "2010-06-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.850000381469727
      },
      {
        "Date": "2010-06-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.989999771118164
      },
      {
        "Date": "2010-06-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.290000915527344
      },
      {
        "Date": "2010-06-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.59000015258789
      },
      {
        "Date": "2010-06-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.1299991607666
      },
      {
        "Date": "2010-06-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.59000015258789
      },
      {"Date": "2010-06-11T00:00:00", "Bank": "MS", "Stock Price": 26},
      {
        "Date": "2010-06-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.329999923706055
      },
      {
        "Date": "2010-06-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.950000762939453
      },
      {
        "Date": "2010-06-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.770000457763672
      },
      {
        "Date": "2010-06-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.31999969482422
      },
      {
        "Date": "2010-06-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.700000762939453
      },
      {
        "Date": "2010-06-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.610000610351562
      },
      {
        "Date": "2010-06-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.18000030517578
      },
      {
        "Date": "2010-06-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.030000686645508
      },
      {
        "Date": "2010-06-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.260000228881836
      },
      {
        "Date": "2010-06-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.010000228881836
      },
      {
        "Date": "2010-06-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.520000457763672
      },
      {
        "Date": "2010-06-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.450000762939453
      },
      {
        "Date": "2010-06-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.209999084472656
      },
      {
        "Date": "2010-07-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.09000015258789
      },
      {
        "Date": "2010-07-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.829999923706055
      },
      {
        "Date": "2010-07-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 22.969999313354492
      },
      {
        "Date": "2010-07-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 23.950000762939453
      },
      {
        "Date": "2010-07-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.200000762939453
      },
      {
        "Date": "2010-07-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.700000762939453
      },
      {
        "Date": "2010-07-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.559999465942383
      },
      {
        "Date": "2010-07-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.65999984741211
      },
      {
        "Date": "2010-07-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.540000915527344
      },
      {
        "Date": "2010-07-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.59000015258789
      },
      {
        "Date": "2010-07-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.739999771118164
      },
      {
        "Date": "2010-07-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.780000686645508
      },
      {
        "Date": "2010-07-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.219999313354492
      },
      {
        "Date": "2010-07-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.799999237060547
      },
      {
        "Date": "2010-07-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.790000915527344
      },
      {
        "Date": "2010-07-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.889999389648438
      },
      {"Date": "2010-07-26T00:00:00", "Bank": "MS", "Stock Price": 27},
      {"Date": "2010-07-27T00:00:00", "Bank": "MS", "Stock Price": 27},
      {
        "Date": "2010-07-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.010000228881836
      },
      {
        "Date": "2010-07-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.989999771118164
      },
      {
        "Date": "2010-07-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.989999771118164
      },
      {
        "Date": "2010-08-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.68000030517578
      },
      {
        "Date": "2010-08-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.489999771118164
      },
      {
        "Date": "2010-08-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.8700008392334
      },
      {
        "Date": "2010-08-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.84000015258789
      },
      {
        "Date": "2010-08-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.649999618530273
      },
      {
        "Date": "2010-08-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.450000762939453
      },
      {
        "Date": "2010-08-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.329999923706055
      },
      {
        "Date": "2010-08-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.43000030517578
      },
      {
        "Date": "2010-08-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.1200008392334
      },
      {
        "Date": "2010-08-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.899999618530273
      },
      {
        "Date": "2010-08-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.700000762939453
      },
      {
        "Date": "2010-08-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.200000762939453
      },
      {
        "Date": "2010-08-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.260000228881836
      },
      {
        "Date": "2010-08-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.989999771118164
      },
      {
        "Date": "2010-08-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.920000076293945
      },
      {
        "Date": "2010-08-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.719999313354492
      },
      {
        "Date": "2010-08-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.1299991607666
      },
      {
        "Date": "2010-08-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.100000381469727
      },
      {
        "Date": "2010-08-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.6299991607666
      },
      {
        "Date": "2010-08-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.030000686645508
      },
      {
        "Date": "2010-08-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.43000030517578
      },
      {
        "Date": "2010-08-31T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.690000534057617
      },
      {
        "Date": "2010-09-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.40999984741211
      },
      {
        "Date": "2010-09-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.68000030517578
      },
      {
        "Date": "2010-09-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.65999984741211
      },
      {
        "Date": "2010-09-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.670000076293945
      },
      {
        "Date": "2010-09-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.969999313354492
      },
      {
        "Date": "2010-09-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.010000228881836
      },
      {
        "Date": "2010-09-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.190000534057617
      },
      {
        "Date": "2010-09-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.770000457763672
      },
      {
        "Date": "2010-09-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.520000457763672
      },
      {
        "Date": "2010-09-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.239999771118164
      },
      {
        "Date": "2010-09-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.780000686645508
      },
      {
        "Date": "2010-09-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.469999313354492
      },
      {
        "Date": "2010-09-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.84000015258789
      },
      {
        "Date": "2010-09-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.059999465942383
      },
      {
        "Date": "2010-09-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.950000762939453
      },
      {
        "Date": "2010-09-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.739999771118164
      },
      {
        "Date": "2010-09-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.149999618530273
      },
      {
        "Date": "2010-09-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.8700008392334
      },
      {"Date": "2010-09-28T00:00:00", "Bank": "MS", "Stock Price": 24.5},
      {
        "Date": "2010-09-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.479999542236328
      },
      {
        "Date": "2010-09-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.68000030517578
      },
      {
        "Date": "2010-10-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.020000457763672
      },
      {
        "Date": "2010-10-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.709999084472656
      },
      {
        "Date": "2010-10-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.469999313354492
      },
      {
        "Date": "2010-10-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.3799991607666
      },
      {
        "Date": "2010-10-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.06999969482422
      },
      {
        "Date": "2010-10-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.31999969482422
      },
      {
        "Date": "2010-10-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.149999618530273
      },
      {
        "Date": "2010-10-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.93000030517578
      },
      {
        "Date": "2010-10-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.940000534057617
      },
      {
        "Date": "2010-10-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.440000534057617
      },
      {
        "Date": "2010-10-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.020000457763672
      },
      {
        "Date": "2010-10-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.399999618530273
      },
      {
        "Date": "2010-10-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.389999389648438
      },
      {
        "Date": "2010-10-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.3799991607666
      },
      {
        "Date": "2010-10-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.600000381469727
      },
      {
        "Date": "2010-10-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.520000457763672
      },
      {
        "Date": "2010-10-25T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.3799991607666
      },
      {
        "Date": "2010-10-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.190000534057617
      },
      {
        "Date": "2010-10-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.399999618530273
      },
      {
        "Date": "2010-10-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.860000610351562
      },
      {
        "Date": "2010-10-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.8700008392334
      },
      {
        "Date": "2010-11-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.68000030517578
      },
      {
        "Date": "2010-11-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.610000610351562
      },
      {
        "Date": "2010-11-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.399999618530273
      },
      {
        "Date": "2010-11-04T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.3700008392334
      },
      {
        "Date": "2010-11-05T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.280000686645508
      },
      {
        "Date": "2010-11-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.209999084472656
      },
      {
        "Date": "2010-11-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.31999969482422
      },
      {
        "Date": "2010-11-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.549999237060547
      },
      {
        "Date": "2010-11-11T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.309999465942383
      },
      {
        "Date": "2010-11-12T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.56999969482422
      },
      {"Date": "2010-11-15T00:00:00", "Bank": "MS", "Stock Price": 26},
      {
        "Date": "2010-11-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.6299991607666
      },
      {
        "Date": "2010-11-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.09000015258789
      },
      {
        "Date": "2010-11-18T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.56999969482422
      },
      {
        "Date": "2010-11-19T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.6200008392334
      },
      {
        "Date": "2010-11-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.059999465942383
      },
      {
        "Date": "2010-11-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.65999984741211
      },
      {
        "Date": "2010-11-24T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.149999618530273
      },
      {
        "Date": "2010-11-26T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.700000762939453
      },
      {
        "Date": "2010-11-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.920000076293945
      },
      {
        "Date": "2010-11-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.459999084472656
      },
      {
        "Date": "2010-12-01T00:00:00",
        "Bank": "MS",
        "Stock Price": 24.920000076293945
      },
      {
        "Date": "2010-12-02T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.610000610351562
      },
      {
        "Date": "2010-12-03T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.639999389648438
      },
      {
        "Date": "2010-12-06T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.540000915527344
      },
      {
        "Date": "2010-12-07T00:00:00",
        "Bank": "MS",
        "Stock Price": 25.65999984741211
      },
      {
        "Date": "2010-12-08T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.469999313354492
      },
      {
        "Date": "2010-12-09T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.709999084472656
      },
      {
        "Date": "2010-12-10T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.950000762939453
      },
      {
        "Date": "2010-12-13T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.940000534057617
      },
      {
        "Date": "2010-12-14T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.6299991607666
      },
      {
        "Date": "2010-12-15T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.200000762939453
      },
      {
        "Date": "2010-12-16T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.010000228881836
      },
      {
        "Date": "2010-12-17T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.239999771118164
      },
      {
        "Date": "2010-12-20T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.260000228881836
      },
      {
        "Date": "2010-12-21T00:00:00",
        "Bank": "MS",
        "Stock Price": 26.860000610351562
      },
      {
        "Date": "2010-12-22T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.399999618530273
      },
      {
        "Date": "2010-12-23T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.40999984741211
      },
      {
        "Date": "2010-12-27T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.510000228881836
      },
      {
        "Date": "2010-12-28T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.65999984741211
      },
      {
        "Date": "2010-12-29T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.280000686645508
      },
      {
        "Date": "2010-12-30T00:00:00",
        "Bank": "MS",
        "Stock Price": 27.329999923706055
      },
      {
        "Date": "2007-01-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.039999961853027
      },
      {
        "Date": "2007-01-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.510000228881836
      },
      {
        "Date": "2007-01-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.140000343322754
      },
      {"Date": "2007-01-08T00:00:00", "Bank": "^VIX", "Stock Price": 12},
      {
        "Date": "2007-01-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.90999984741211
      },
      {
        "Date": "2007-01-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.470000267028809
      },
      {
        "Date": "2007-01-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.869999885559082
      },
      {
        "Date": "2007-01-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.149999618530273
      },
      {
        "Date": "2007-01-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.739999771118164
      },
      {
        "Date": "2007-01-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.59000015258789
      },
      {
        "Date": "2007-01-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.850000381469727
      },
      {
        "Date": "2007-01-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.399999618530273
      },
      {
        "Date": "2007-01-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.770000457763672
      },
      {
        "Date": "2007-01-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.34000015258789
      },
      {
        "Date": "2007-01-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 9.890000343322754
      },
      {
        "Date": "2007-01-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.220000267028809
      },
      {
        "Date": "2007-01-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.130000114440918
      },
      {
        "Date": "2007-01-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.449999809265137
      },
      {
        "Date": "2007-01-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.960000038146973
      },
      {
        "Date": "2007-01-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.420000076293945
      },
      {
        "Date": "2007-02-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.3100004196167
      },
      {
        "Date": "2007-02-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.079999923706055
      },
      {
        "Date": "2007-02-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.550000190734863
      },
      {
        "Date": "2007-02-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.649999618530273
      },
      {
        "Date": "2007-02-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.319999694824219
      },
      {
        "Date": "2007-02-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.4399995803833
      },
      {
        "Date": "2007-02-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.100000381469727
      },
      {
        "Date": "2007-02-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.609999656677246
      },
      {
        "Date": "2007-02-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.34000015258789
      },
      {
        "Date": "2007-02-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.229999542236328
      },
      {
        "Date": "2007-02-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.220000267028809
      },
      {
        "Date": "2007-02-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.020000457763672
      },
      {
        "Date": "2007-02-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.239999771118164
      },
      {
        "Date": "2007-02-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.199999809265137
      },
      {
        "Date": "2007-02-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.180000305175781
      },
      {
        "Date": "2007-02-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 10.579999923706055
      },
      {
        "Date": "2007-02-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.149999618530273
      },
      {
        "Date": "2007-02-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.309999465942383
      },
      {
        "Date": "2007-02-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.420000076293945
      },
      {
        "Date": "2007-03-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.819999694824219
      },
      {
        "Date": "2007-03-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.610000610351562
      },
      {
        "Date": "2007-03-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.6299991607666
      },
      {
        "Date": "2007-03-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.960000038146973
      },
      {
        "Date": "2007-03-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.239999771118164
      },
      {
        "Date": "2007-03-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.289999961853027
      },
      {
        "Date": "2007-03-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.09000015258789
      },
      {
        "Date": "2007-03-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.989999771118164
      },
      {
        "Date": "2007-03-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.1299991607666
      },
      {
        "Date": "2007-03-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.270000457763672
      },
      {
        "Date": "2007-03-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.43000030517578
      },
      {
        "Date": "2007-03-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.790000915527344
      },
      {
        "Date": "2007-03-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.59000015258789
      },
      {
        "Date": "2007-03-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.270000457763672
      },
      {
        "Date": "2007-03-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.1899995803833
      },
      {
        "Date": "2007-03-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.930000305175781
      },
      {
        "Date": "2007-03-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.949999809265137
      },
      {
        "Date": "2007-03-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.15999984741211
      },
      {
        "Date": "2007-03-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.479999542236328
      },
      {
        "Date": "2007-03-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.979999542236328
      },
      {
        "Date": "2007-03-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.140000343322754
      },
      {
        "Date": "2007-03-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.640000343322754
      },
      {
        "Date": "2007-04-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.529999732971191
      },
      {
        "Date": "2007-04-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.460000038146973
      },
      {
        "Date": "2007-04-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.239999771118164
      },
      {
        "Date": "2007-04-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.229999542236328
      },
      {
        "Date": "2007-04-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.140000343322754
      },
      {
        "Date": "2007-04-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.680000305175781
      },
      {
        "Date": "2007-04-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.489999771118164
      },
      {
        "Date": "2007-04-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.710000038146973
      },
      {
        "Date": "2007-04-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.199999809265137
      },
      {
        "Date": "2007-04-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 11.979999542236328
      },
      {
        "Date": "2007-04-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.140000343322754
      },
      {
        "Date": "2007-04-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.420000076293945
      },
      {
        "Date": "2007-04-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.539999961853027
      },
      {
        "Date": "2007-04-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.069999694824219
      },
      {
        "Date": "2007-04-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.039999961853027
      },
      {
        "Date": "2007-04-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.119999885559082
      },
      {
        "Date": "2007-04-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.210000038146973
      },
      {
        "Date": "2007-04-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.789999961853027
      },
      {
        "Date": "2007-04-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.449999809265137
      },
      {
        "Date": "2007-04-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.220000267028809
      },
      {
        "Date": "2007-05-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.510000228881836
      },
      {
        "Date": "2007-05-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.079999923706055
      },
      {
        "Date": "2007-05-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.09000015258789
      },
      {
        "Date": "2007-05-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.90999984741211
      },
      {
        "Date": "2007-05-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.149999618530273
      },
      {
        "Date": "2007-05-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.210000038146973
      },
      {
        "Date": "2007-05-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.880000114440918
      },
      {
        "Date": "2007-05-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.600000381469727
      },
      {
        "Date": "2007-05-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.949999809265137
      },
      {
        "Date": "2007-05-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.960000038146973
      },
      {
        "Date": "2007-05-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.010000228881836
      },
      {"Date": "2007-05-16T00:00:00", "Bank": "^VIX", "Stock Price": 13.5},
      {
        "Date": "2007-05-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.510000228881836
      },
      {
        "Date": "2007-05-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.760000228881836
      },
      {
        "Date": "2007-05-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.300000190734863
      },
      {
        "Date": "2007-05-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.0600004196167
      },
      {
        "Date": "2007-05-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.239999771118164
      },
      {
        "Date": "2007-05-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.079999923706055
      },
      {
        "Date": "2007-05-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.34000015258789
      },
      {
        "Date": "2007-05-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.529999732971191
      },
      {
        "Date": "2007-05-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.829999923706055
      },
      {
        "Date": "2007-05-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.050000190734863
      },
      {
        "Date": "2007-06-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.779999732971191
      },
      {
        "Date": "2007-06-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.289999961853027
      },
      {
        "Date": "2007-06-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.630000114440918
      },
      {
        "Date": "2007-06-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.869999885559082
      },
      {
        "Date": "2007-06-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.059999465942383
      },
      {
        "Date": "2007-06-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.84000015258789
      },
      {
        "Date": "2007-06-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.710000038146973
      },
      {
        "Date": "2007-06-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.670000076293945
      },
      {
        "Date": "2007-06-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.729999542236328
      },
      {
        "Date": "2007-06-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.640000343322754
      },
      {
        "Date": "2007-06-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.9399995803833
      },
      {
        "Date": "2007-06-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 13.420000076293945
      },
      {
        "Date": "2007-06-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 12.850000381469727
      },
      {
        "Date": "2007-06-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.670000076293945
      },
      {
        "Date": "2007-06-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.210000038146973
      },
      {"Date": "2007-06-22T00:00:00", "Bank": "^VIX", "Stock Price": 15.75},
      {
        "Date": "2007-06-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.649999618530273
      },
      {
        "Date": "2007-06-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.889999389648438
      },
      {
        "Date": "2007-06-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.529999732971191
      },
      {
        "Date": "2007-06-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.539999961853027
      },
      {
        "Date": "2007-06-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.229999542236328
      },
      {
        "Date": "2007-07-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.399999618530273
      },
      {
        "Date": "2007-07-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.920000076293945
      },
      {
        "Date": "2007-07-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.479999542236328
      },
      {
        "Date": "2007-07-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 14.720000267028809
      },
      {
        "Date": "2007-07-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.15999984741211
      },
      {
        "Date": "2007-07-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.56999969482422
      },
      {
        "Date": "2007-07-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.639999389648438
      },
      {
        "Date": "2007-07-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.539999961853027
      },
      {
        "Date": "2007-07-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.149999618530273
      },
      {
        "Date": "2007-07-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.59000015258789
      },
      {
        "Date": "2007-07-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.630000114440918
      },
      {"Date": "2007-07-18T00:00:00", "Bank": "^VIX", "Stock Price": 16},
      {
        "Date": "2007-07-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.229999542236328
      },
      {
        "Date": "2007-07-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.950000762939453
      },
      {
        "Date": "2007-07-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.809999465942383
      },
      {
        "Date": "2007-07-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.549999237060547
      },
      {
        "Date": "2007-07-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.100000381469727
      },
      {
        "Date": "2007-07-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.739999771118164
      },
      {
        "Date": "2007-07-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.170000076293945
      },
      {
        "Date": "2007-07-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.8700008392334
      },
      {
        "Date": "2007-07-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.520000457763672
      },
      {
        "Date": "2007-08-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.670000076293945
      },
      {
        "Date": "2007-08-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.219999313354492
      },
      {
        "Date": "2007-08-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.15999984741211
      },
      {
        "Date": "2007-08-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.940000534057617
      },
      {
        "Date": "2007-08-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.559999465942383
      },
      {
        "Date": "2007-08-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.450000762939453
      },
      {
        "Date": "2007-08-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.479999542236328
      },
      {
        "Date": "2007-08-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.299999237060547
      },
      {
        "Date": "2007-08-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.56999969482422
      },
      {
        "Date": "2007-08-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.68000030517578
      },
      {
        "Date": "2007-08-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.670000076293945
      },
      {
        "Date": "2007-08-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.829999923706055
      },
      {
        "Date": "2007-08-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.989999771118164
      },
      {
        "Date": "2007-08-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.329999923706055
      },
      {"Date": "2007-08-21T00:00:00", "Bank": "^VIX", "Stock Price": 25.25},
      {
        "Date": "2007-08-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.889999389648438
      },
      {
        "Date": "2007-08-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.6200008392334
      },
      {
        "Date": "2007-08-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.719999313354492
      },
      {
        "Date": "2007-08-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.719999313354492
      },
      {
        "Date": "2007-08-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.299999237060547
      },
      {
        "Date": "2007-08-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.809999465942383
      },
      {
        "Date": "2007-08-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.059999465942383
      },
      {
        "Date": "2007-08-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.3799991607666
      },
      {
        "Date": "2007-09-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.780000686645508
      },
      {
        "Date": "2007-09-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.579999923706055
      },
      {
        "Date": "2007-09-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.989999771118164
      },
      {
        "Date": "2007-09-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.229999542236328
      },
      {
        "Date": "2007-09-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.3799991607666
      },
      {
        "Date": "2007-09-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.270000457763672
      },
      {
        "Date": "2007-09-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.959999084472656
      },
      {
        "Date": "2007-09-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.760000228881836
      },
      {
        "Date": "2007-09-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.920000076293945
      },
      {
        "Date": "2007-09-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.479999542236328
      },
      {
        "Date": "2007-09-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.350000381469727
      },
      {
        "Date": "2007-09-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.030000686645508
      },
      {
        "Date": "2007-09-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.450000762939453
      },
      {"Date": "2007-09-21T00:00:00", "Bank": "^VIX", "Stock Price": 19},
      {
        "Date": "2007-09-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.3700008392334
      },
      {
        "Date": "2007-09-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.600000381469727
      },
      {
        "Date": "2007-09-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.6299991607666
      },
      {"Date": "2007-09-27T00:00:00", "Bank": "^VIX", "Stock Price": 17},
      {"Date": "2007-09-28T00:00:00", "Bank": "^VIX", "Stock Price": 18},
      {
        "Date": "2007-10-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.84000015258789
      },
      {
        "Date": "2007-10-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.489999771118164
      },
      {
        "Date": "2007-10-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.799999237060547
      },
      {
        "Date": "2007-10-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.440000534057617
      },
      {
        "Date": "2007-10-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.90999984741211
      },
      {
        "Date": "2007-10-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.459999084472656
      },
      {
        "Date": "2007-10-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.1200008392334
      },
      {
        "Date": "2007-10-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.670000076293945
      },
      {
        "Date": "2007-10-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.8799991607666
      },
      {
        "Date": "2007-10-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.729999542236328
      },
      {"Date": "2007-10-15T00:00:00", "Bank": "^VIX", "Stock Price": 19.25},
      {
        "Date": "2007-10-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.020000457763672
      },
      {
        "Date": "2007-10-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.540000915527344
      },
      {"Date": "2007-10-18T00:00:00", "Bank": "^VIX", "Stock Price": 18.5},
      {
        "Date": "2007-10-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.959999084472656
      },
      {
        "Date": "2007-10-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.639999389648438
      },
      {
        "Date": "2007-10-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.40999984741211
      },
      {
        "Date": "2007-10-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.799999237060547
      },
      {
        "Date": "2007-10-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.170000076293945
      },
      {
        "Date": "2007-10-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.559999465942383
      },
      {
        "Date": "2007-10-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.8700008392334
      },
      {
        "Date": "2007-10-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.06999969482422
      },
      {
        "Date": "2007-10-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.530000686645508
      },
      {
        "Date": "2007-11-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.209999084472656
      },
      {
        "Date": "2007-11-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.010000228881836
      },
      {
        "Date": "2007-11-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.309999465942383
      },
      {
        "Date": "2007-11-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.389999389648438
      },
      {
        "Date": "2007-11-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.489999771118164
      },
      {
        "Date": "2007-11-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.15999984741211
      },
      {"Date": "2007-11-09T00:00:00", "Bank": "^VIX", "Stock Price": 28.5},
      {
        "Date": "2007-11-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.09000015258789
      },
      {
        "Date": "2007-11-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.100000381469727
      },
      {
        "Date": "2007-11-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.940000534057617
      },
      {
        "Date": "2007-11-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.059999465942383
      },
      {
        "Date": "2007-11-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.489999771118164
      },
      {
        "Date": "2007-11-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.010000228881836
      },
      {
        "Date": "2007-11-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.8799991607666
      },
      {
        "Date": "2007-11-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.84000015258789
      },
      {
        "Date": "2007-11-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.610000610351562
      },
      {
        "Date": "2007-11-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.90999984741211
      },
      {
        "Date": "2007-11-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.280000686645508
      },
      {
        "Date": "2007-11-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.110000610351562
      },
      {
        "Date": "2007-11-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.969999313354492
      },
      {
        "Date": "2007-11-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.8700008392334
      },
      {
        "Date": "2007-12-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.610000610351562
      },
      {
        "Date": "2007-12-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.790000915527344
      },
      {
        "Date": "2007-12-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.530000686645508
      },
      {
        "Date": "2007-12-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.959999084472656
      },
      {
        "Date": "2007-12-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.850000381469727
      },
      {
        "Date": "2007-12-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.739999771118164
      },
      {
        "Date": "2007-12-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.59000015258789
      },
      {
        "Date": "2007-12-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.469999313354492
      },
      {
        "Date": "2007-12-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.559999465942383
      },
      {
        "Date": "2007-12-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.270000457763672
      },
      {
        "Date": "2007-12-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.520000457763672
      },
      {
        "Date": "2007-12-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.639999389648438
      },
      {
        "Date": "2007-12-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.68000030517578
      },
      {
        "Date": "2007-12-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.579999923706055
      },
      {
        "Date": "2007-12-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.469999313354492
      },
      {
        "Date": "2007-12-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.600000381469727
      },
      {
        "Date": "2007-12-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.65999984741211
      },
      {
        "Date": "2007-12-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.260000228881836
      },
      {
        "Date": "2007-12-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.739999771118164
      },
      {"Date": "2007-12-31T00:00:00", "Bank": "^VIX", "Stock Price": 22.5},
      {
        "Date": "2008-01-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.170000076293945
      },
      {
        "Date": "2008-01-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.489999771118164
      },
      {
        "Date": "2008-01-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.940000534057617
      },
      {
        "Date": "2008-01-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.790000915527344
      },
      {
        "Date": "2008-01-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.43000030517578
      },
      {
        "Date": "2008-01-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.1200008392334
      },
      {
        "Date": "2008-01-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.450000762939453
      },
      {
        "Date": "2008-01-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.68000030517578
      },
      {
        "Date": "2008-01-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.899999618530273
      },
      {
        "Date": "2008-01-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.34000015258789
      },
      {
        "Date": "2008-01-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.3799991607666
      },
      {
        "Date": "2008-01-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.459999084472656
      },
      {
        "Date": "2008-01-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.18000030517578
      },
      {
        "Date": "2008-01-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.010000228881836
      },
      {
        "Date": "2008-01-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.020000457763672
      },
      {
        "Date": "2008-01-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.780000686645508
      },
      {
        "Date": "2008-01-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.079999923706055
      },
      {
        "Date": "2008-01-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.780000686645508
      },
      {
        "Date": "2008-01-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.31999969482422
      },
      {
        "Date": "2008-01-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.6200008392334
      },
      {
        "Date": "2008-01-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.200000762939453
      },
      {
        "Date": "2008-02-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.020000457763672
      },
      {
        "Date": "2008-02-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.989999771118164
      },
      {
        "Date": "2008-02-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.239999771118164
      },
      {
        "Date": "2008-02-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.969999313354492
      },
      {
        "Date": "2008-02-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.65999984741211
      },
      {
        "Date": "2008-02-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.010000228881836
      },
      {
        "Date": "2008-02-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.600000381469727
      },
      {
        "Date": "2008-02-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.329999923706055
      },
      {
        "Date": "2008-02-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.8799991607666
      },
      {
        "Date": "2008-02-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.540000915527344
      },
      {
        "Date": "2008-02-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.020000457763672
      },
      {
        "Date": "2008-02-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.59000015258789
      },
      {
        "Date": "2008-02-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.399999618530273
      },
      {
        "Date": "2008-02-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.1200008392334
      },
      {
        "Date": "2008-02-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.059999465942383
      },
      {
        "Date": "2008-02-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.030000686645508
      },
      {
        "Date": "2008-02-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.899999618530273
      },
      {
        "Date": "2008-02-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.690000534057617
      },
      {
        "Date": "2008-02-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.530000686645508
      },
      {
        "Date": "2008-02-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.540000915527344
      },
      {
        "Date": "2008-03-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.280000686645508
      },
      {
        "Date": "2008-03-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.520000457763672
      },
      {
        "Date": "2008-03-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.600000381469727
      },
      {
        "Date": "2008-03-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.549999237060547
      },
      {
        "Date": "2008-03-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.489999771118164
      },
      {
        "Date": "2008-03-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.3799991607666
      },
      {
        "Date": "2008-03-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.360000610351562
      },
      {
        "Date": "2008-03-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.219999313354492
      },
      {
        "Date": "2008-03-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.290000915527344
      },
      {
        "Date": "2008-03-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.15999984741211
      },
      {
        "Date": "2008-03-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.2400016784668
      },
      {
        "Date": "2008-03-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.790000915527344
      },
      {
        "Date": "2008-03-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.84000015258789
      },
      {
        "Date": "2008-03-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.6200008392334
      },
      {
        "Date": "2008-03-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.729999542236328
      },
      {
        "Date": "2008-03-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.719999313354492
      },
      {
        "Date": "2008-03-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.079999923706055
      },
      {
        "Date": "2008-03-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.8799991607666
      },
      {
        "Date": "2008-03-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.709999084472656
      },
      {
        "Date": "2008-03-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.610000610351562
      },
      {
        "Date": "2008-04-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.68000030517578
      },
      {
        "Date": "2008-04-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.43000030517578
      },
      {
        "Date": "2008-04-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.209999084472656
      },
      {
        "Date": "2008-04-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.450000762939453
      },
      {
        "Date": "2008-04-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.420000076293945
      },
      {
        "Date": "2008-04-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.360000610351562
      },
      {
        "Date": "2008-04-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.809999465942383
      },
      {
        "Date": "2008-04-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.979999542236328
      },
      {
        "Date": "2008-04-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.459999084472656
      },
      {
        "Date": "2008-04-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.81999969482422
      },
      {
        "Date": "2008-04-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.780000686645508
      },
      {
        "Date": "2008-04-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.530000686645508
      },
      {
        "Date": "2008-04-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.3700008392334
      },
      {
        "Date": "2008-04-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.1299991607666
      },
      {"Date": "2008-04-21T00:00:00", "Bank": "^VIX", "Stock Price": 20.5},
      {
        "Date": "2008-04-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.8700008392334
      },
      {
        "Date": "2008-04-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.260000228881836
      },
      {
        "Date": "2008-04-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.059999465942383
      },
      {
        "Date": "2008-04-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.59000015258789
      },
      {
        "Date": "2008-04-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.639999389648438
      },
      {
        "Date": "2008-04-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.239999771118164
      },
      {
        "Date": "2008-04-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.790000915527344
      },
      {
        "Date": "2008-05-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.8799991607666
      },
      {
        "Date": "2008-05-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.18000030517578
      },
      {
        "Date": "2008-05-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.899999618530273
      },
      {
        "Date": "2008-05-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.209999084472656
      },
      {
        "Date": "2008-05-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.729999542236328
      },
      {
        "Date": "2008-05-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.399999618530273
      },
      {
        "Date": "2008-05-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.40999984741211
      },
      {
        "Date": "2008-05-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.790000915527344
      },
      {
        "Date": "2008-05-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.979999542236328
      },
      {
        "Date": "2008-05-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.65999984741211
      },
      {
        "Date": "2008-05-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.299999237060547
      },
      {
        "Date": "2008-05-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.469999313354492
      },
      {
        "Date": "2008-05-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.010000228881836
      },
      {
        "Date": "2008-05-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.579999923706055
      },
      {
        "Date": "2008-05-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.59000015258789
      },
      {
        "Date": "2008-05-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.049999237060547
      },
      {
        "Date": "2008-05-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.549999237060547
      },
      {
        "Date": "2008-05-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.639999389648438
      },
      {
        "Date": "2008-05-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.06999969482422
      },
      {
        "Date": "2008-05-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.139999389648438
      },
      {
        "Date": "2008-05-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.829999923706055
      },
      {
        "Date": "2008-06-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.829999923706055
      },
      {
        "Date": "2008-06-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.239999771118164
      },
      {
        "Date": "2008-06-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.799999237060547
      },
      {
        "Date": "2008-06-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.6299991607666
      },
      {
        "Date": "2008-06-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.559999465942383
      },
      {
        "Date": "2008-06-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.1200008392334
      },
      {
        "Date": "2008-06-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.18000030517578
      },
      {
        "Date": "2008-06-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.1200008392334
      },
      {
        "Date": "2008-06-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.329999923706055
      },
      {
        "Date": "2008-06-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.219999313354492
      },
      {
        "Date": "2008-06-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.950000762939453
      },
      {
        "Date": "2008-06-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.1299991607666
      },
      {
        "Date": "2008-06-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.239999771118164
      },
      {
        "Date": "2008-06-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.579999923706055
      },
      {
        "Date": "2008-06-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.8700008392334
      },
      {
        "Date": "2008-06-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.639999389648438
      },
      {
        "Date": "2008-06-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.420000076293945
      },
      {
        "Date": "2008-06-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.139999389648438
      },
      {
        "Date": "2008-06-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.93000030517578
      },
      {
        "Date": "2008-06-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.440000534057617
      },
      {
        "Date": "2008-06-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.950000762939453
      },
      {
        "Date": "2008-07-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.649999618530273
      },
      {
        "Date": "2008-07-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.920000076293945
      },
      {
        "Date": "2008-07-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.780000686645508
      },
      {
        "Date": "2008-07-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.780000686645508
      },
      {
        "Date": "2008-07-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.149999618530273
      },
      {
        "Date": "2008-07-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.229999542236328
      },
      {
        "Date": "2008-07-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.59000015258789
      },
      {
        "Date": "2008-07-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.489999771118164
      },
      {
        "Date": "2008-07-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.479999542236328
      },
      {
        "Date": "2008-07-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.540000915527344
      },
      {
        "Date": "2008-07-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.100000381469727
      },
      {
        "Date": "2008-07-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.010000228881836
      },
      {
        "Date": "2008-07-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.049999237060547
      },
      {
        "Date": "2008-07-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.049999237060547
      },
      {
        "Date": "2008-07-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.18000030517578
      },
      {
        "Date": "2008-07-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.309999465942383
      },
      {
        "Date": "2008-07-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.440000534057617
      },
      {
        "Date": "2008-07-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.90999984741211
      },
      {
        "Date": "2008-07-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.229999542236328
      },
      {
        "Date": "2008-07-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.030000686645508
      },
      {
        "Date": "2008-07-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.209999084472656
      },
      {
        "Date": "2008-07-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.940000534057617
      },
      {
        "Date": "2008-08-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.56999969482422
      },
      {
        "Date": "2008-08-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.489999771118164
      },
      {
        "Date": "2008-08-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.139999389648438
      },
      {
        "Date": "2008-08-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.229999542236328
      },
      {
        "Date": "2008-08-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.149999618530273
      },
      {
        "Date": "2008-08-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.65999984741211
      },
      {
        "Date": "2008-08-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.1200008392334
      },
      {
        "Date": "2008-08-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.170000076293945
      },
      {
        "Date": "2008-08-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.549999237060547
      },
      {
        "Date": "2008-08-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.34000015258789
      },
      {
        "Date": "2008-08-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.579999923706055
      },
      {
        "Date": "2008-08-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.979999542236328
      },
      {
        "Date": "2008-08-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.280000686645508
      },
      {
        "Date": "2008-08-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.420000076293945
      },
      {
        "Date": "2008-08-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.81999969482422
      },
      {
        "Date": "2008-08-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.809999465942383
      },
      {
        "Date": "2008-08-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.969999313354492
      },
      {
        "Date": "2008-08-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.489999771118164
      },
      {
        "Date": "2008-08-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.760000228881836
      },
      {
        "Date": "2008-08-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.43000030517578
      },
      {
        "Date": "2008-08-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.649999618530273
      },
      {
        "Date": "2008-09-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.989999771118164
      },
      {
        "Date": "2008-09-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.43000030517578
      },
      {
        "Date": "2008-09-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.030000686645508
      },
      {
        "Date": "2008-09-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.059999465942383
      },
      {
        "Date": "2008-09-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.639999389648438
      },
      {
        "Date": "2008-09-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.469999313354492
      },
      {
        "Date": "2008-09-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.520000457763672
      },
      {
        "Date": "2008-09-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.389999389648438
      },
      {
        "Date": "2008-09-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.65999984741211
      },
      {
        "Date": "2008-09-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.700000762939453
      },
      {
        "Date": "2008-09-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.299999237060547
      },
      {
        "Date": "2008-09-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 36.220001220703125
      },
      {
        "Date": "2008-09-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.099998474121094
      },
      {
        "Date": "2008-09-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.06999969482422
      },
      {
        "Date": "2008-09-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.849998474121094
      },
      {
        "Date": "2008-09-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.720001220703125
      },
      {
        "Date": "2008-09-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.189998626708984
      },
      {
        "Date": "2008-09-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.81999969482422
      },
      {
        "Date": "2008-09-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 34.7400016784668
      },
      {
        "Date": "2008-09-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 46.720001220703125
      },
      {
        "Date": "2008-09-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 39.38999938964844
      },
      {
        "Date": "2008-10-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 39.810001373291016
      },
      {
        "Date": "2008-10-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.2599983215332
      },
      {
        "Date": "2008-10-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.13999938964844
      },
      {
        "Date": "2008-10-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 52.04999923706055
      },
      {
        "Date": "2008-10-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 53.68000030517578
      },
      {
        "Date": "2008-10-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 57.529998779296875
      },
      {
        "Date": "2008-10-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 63.91999816894531
      },
      {
        "Date": "2008-10-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 69.94999694824219
      },
      {
        "Date": "2008-10-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 54.9900016784668
      },
      {
        "Date": "2008-10-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 55.130001068115234
      },
      {"Date": "2008-10-15T00:00:00", "Bank": "^VIX", "Stock Price": 69.25},
      {
        "Date": "2008-10-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 67.61000061035156
      },
      {
        "Date": "2008-10-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 70.33000183105469
      },
      {
        "Date": "2008-10-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 52.970001220703125
      },
      {
        "Date": "2008-10-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 53.11000061035156
      },
      {
        "Date": "2008-10-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 69.6500015258789
      },
      {
        "Date": "2008-10-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 67.80000305175781
      },
      {
        "Date": "2008-10-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 79.12999725341797
      },
      {
        "Date": "2008-10-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 80.05999755859375
      },
      {
        "Date": "2008-10-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 66.95999908447266
      },
      {
        "Date": "2008-10-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 69.95999908447266
      },
      {
        "Date": "2008-10-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 62.900001525878906
      },
      {
        "Date": "2008-10-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 59.88999938964844
      },
      {
        "Date": "2008-11-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 53.68000030517578
      },
      {
        "Date": "2008-11-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 47.72999954223633
      },
      {
        "Date": "2008-11-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 54.560001373291016
      },
      {
        "Date": "2008-11-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 63.68000030517578
      },
      {
        "Date": "2008-11-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 56.099998474121094
      },
      {
        "Date": "2008-11-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 59.97999954223633
      },
      {
        "Date": "2008-11-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 61.439998626708984
      },
      {
        "Date": "2008-11-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 66.45999908447266
      },
      {
        "Date": "2008-11-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 59.83000183105469
      },
      {
        "Date": "2008-11-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 66.30999755859375
      },
      {
        "Date": "2008-11-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 69.1500015258789
      },
      {
        "Date": "2008-11-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 67.63999938964844
      },
      {
        "Date": "2008-11-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 74.26000213623047
      },
      {
        "Date": "2008-11-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 80.86000061035156
      },
      {
        "Date": "2008-11-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 72.66999816894531
      },
      {
        "Date": "2008-11-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 64.69999694824219
      },
      {
        "Date": "2008-11-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 60.900001525878906
      },
      {
        "Date": "2008-11-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 54.91999816894531
      },
      {
        "Date": "2008-11-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 55.279998779296875
      },
      {
        "Date": "2008-12-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 68.51000213623047
      },
      {
        "Date": "2008-12-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 62.97999954223633
      },
      {
        "Date": "2008-12-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 60.720001220703125
      },
      {
        "Date": "2008-12-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 63.63999938964844
      },
      {
        "Date": "2008-12-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 59.93000030517578
      },
      {
        "Date": "2008-12-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 58.4900016784668
      },
      {
        "Date": "2008-12-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 58.90999984741211
      },
      {
        "Date": "2008-12-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 55.72999954223633
      },
      {
        "Date": "2008-12-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 55.779998779296875
      },
      {
        "Date": "2008-12-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 54.279998779296875
      },
      {
        "Date": "2008-12-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 56.7599983215332
      },
      {
        "Date": "2008-12-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 52.369998931884766
      },
      {
        "Date": "2008-12-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 49.84000015258789
      },
      {
        "Date": "2008-12-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 47.34000015258789
      },
      {
        "Date": "2008-12-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.93000030517578
      },
      {
        "Date": "2008-12-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.560001373291016
      },
      {
        "Date": "2008-12-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.02000045776367
      },
      {
        "Date": "2008-12-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.209999084472656
      },
      {
        "Date": "2008-12-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.380001068115234
      },
      {
        "Date": "2008-12-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.900001525878906
      },
      {
        "Date": "2008-12-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 41.630001068115234
      },
      {"Date": "2008-12-31T00:00:00", "Bank": "^VIX", "Stock Price": 40},
      {
        "Date": "2009-01-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 39.189998626708984
      },
      {
        "Date": "2009-01-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 39.08000183105469
      },
      {
        "Date": "2009-01-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 38.560001373291016
      },
      {
        "Date": "2009-01-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.38999938964844
      },
      {
        "Date": "2009-01-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.560001373291016
      },
      {
        "Date": "2009-01-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.81999969482422
      },
      {
        "Date": "2009-01-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.84000015258789
      },
      {
        "Date": "2009-01-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.27000045776367
      },
      {
        "Date": "2009-01-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 49.13999938964844
      },
      {"Date": "2009-01-15T00:00:00", "Bank": "^VIX", "Stock Price": 51},
      {
        "Date": "2009-01-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 46.11000061035156
      },
      {
        "Date": "2009-01-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 56.650001525878906
      },
      {
        "Date": "2009-01-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 46.41999816894531
      },
      {
        "Date": "2009-01-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 47.290000915527344
      },
      {
        "Date": "2009-01-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 47.27000045776367
      },
      {
        "Date": "2009-01-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.689998626708984
      },
      {"Date": "2009-01-27T00:00:00", "Bank": "^VIX", "Stock Price": 42.25},
      {
        "Date": "2009-01-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 39.65999984741211
      },
      {
        "Date": "2009-01-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.630001068115234
      },
      {
        "Date": "2009-01-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.84000015258789
      },
      {
        "Date": "2009-02-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.52000045776367
      },
      {
        "Date": "2009-02-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.060001373291016
      },
      {
        "Date": "2009-02-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.849998474121094
      },
      {
        "Date": "2009-02-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.72999954223633
      },
      {
        "Date": "2009-02-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.369998931884766
      },
      {
        "Date": "2009-02-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.63999938964844
      },
      {
        "Date": "2009-02-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 46.66999816894531
      },
      {
        "Date": "2009-02-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.529998779296875
      },
      {"Date": "2009-02-12T00:00:00", "Bank": "^VIX", "Stock Price": 41.25},
      {
        "Date": "2009-02-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.93000030517578
      },
      {
        "Date": "2009-02-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 48.65999984741211
      },
      {
        "Date": "2009-02-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 48.459999084472656
      },
      {
        "Date": "2009-02-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 47.08000183105469
      },
      {
        "Date": "2009-02-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 49.29999923706055
      },
      {
        "Date": "2009-02-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 52.619998931884766
      },
      {
        "Date": "2009-02-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.4900016784668
      },
      {
        "Date": "2009-02-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.66999816894531
      },
      {
        "Date": "2009-02-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.65999984741211
      },
      {
        "Date": "2009-02-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 46.349998474121094
      },
      {
        "Date": "2009-03-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 52.650001525878906
      },
      {
        "Date": "2009-03-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 50.93000030517578
      },
      {
        "Date": "2009-03-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 47.560001373291016
      },
      {
        "Date": "2009-03-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 50.16999816894531
      },
      {
        "Date": "2009-03-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 49.33000183105469
      },
      {
        "Date": "2009-03-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 49.68000030517578
      },
      {
        "Date": "2009-03-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.369998931884766
      },
      {
        "Date": "2009-03-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.61000061035156
      },
      {
        "Date": "2009-03-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 41.18000030517578
      },
      {
        "Date": "2009-03-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.36000061035156
      },
      {
        "Date": "2009-03-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.7400016784668
      },
      {
        "Date": "2009-03-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 40.79999923706055
      },
      {
        "Date": "2009-03-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 40.060001373291016
      },
      {
        "Date": "2009-03-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.68000030517578
      },
      {
        "Date": "2009-03-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.88999938964844
      },
      {
        "Date": "2009-03-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 43.22999954223633
      },
      {
        "Date": "2009-03-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.93000030517578
      },
      {"Date": "2009-03-25T00:00:00", "Bank": "^VIX", "Stock Price": 42.25},
      {
        "Date": "2009-03-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 40.36000061035156
      },
      {
        "Date": "2009-03-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 41.040000915527344
      },
      {
        "Date": "2009-03-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.540000915527344
      },
      {
        "Date": "2009-03-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 44.13999938964844
      },
      {
        "Date": "2009-04-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.279998779296875
      },
      {
        "Date": "2009-04-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 42.040000915527344
      },
      {
        "Date": "2009-04-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 39.70000076293945
      },
      {
        "Date": "2009-04-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 40.93000030517578
      },
      {
        "Date": "2009-04-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 40.38999938964844
      },
      {
        "Date": "2009-04-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 38.849998474121094
      },
      {
        "Date": "2009-04-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 36.529998779296875
      },
      {
        "Date": "2009-04-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 37.810001373291016
      },
      {
        "Date": "2009-04-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 37.66999816894531
      },
      {
        "Date": "2009-04-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 36.16999816894531
      },
      {
        "Date": "2009-04-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.790000915527344
      },
      {
        "Date": "2009-04-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.939998626708984
      },
      {
        "Date": "2009-04-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 39.18000030517578
      },
      {
        "Date": "2009-04-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 37.13999938964844
      },
      {
        "Date": "2009-04-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 38.099998474121094
      },
      {
        "Date": "2009-04-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 37.150001525878906
      },
      {
        "Date": "2009-04-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 36.81999969482422
      },
      {
        "Date": "2009-04-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 38.31999969482422
      },
      {
        "Date": "2009-04-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 37.95000076293945
      },
      {
        "Date": "2009-04-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 36.08000183105469
      },
      {"Date": "2009-04-30T00:00:00", "Bank": "^VIX", "Stock Price": 36.5},
      {
        "Date": "2009-05-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.29999923706055
      },
      {
        "Date": "2009-05-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 34.529998779296875
      },
      {
        "Date": "2009-05-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.36000061035156
      },
      {
        "Date": "2009-05-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.45000076293945
      },
      {
        "Date": "2009-05-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.439998626708984
      },
      {
        "Date": "2009-05-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.04999923706055
      },
      {
        "Date": "2009-05-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.869998931884766
      },
      {
        "Date": "2009-05-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.799999237060547
      },
      {
        "Date": "2009-05-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.650001525878906
      },
      {
        "Date": "2009-05-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.3700008392334
      },
      {
        "Date": "2009-05-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.119998931884766
      },
      {
        "Date": "2009-05-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.239999771118164
      },
      {
        "Date": "2009-05-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.799999237060547
      },
      {
        "Date": "2009-05-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.030000686645508
      },
      {
        "Date": "2009-05-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.350000381469727
      },
      {
        "Date": "2009-05-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.630001068115234
      },
      {
        "Date": "2009-05-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.6200008392334
      },
      {
        "Date": "2009-05-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.36000061035156
      },
      {
        "Date": "2009-05-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.670000076293945
      },
      {
        "Date": "2009-05-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.920000076293945
      },
      {
        "Date": "2009-06-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.040000915527344
      },
      {
        "Date": "2009-06-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.6299991607666
      },
      {
        "Date": "2009-06-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.020000457763672
      },
      {
        "Date": "2009-06-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.18000030517578
      },
      {
        "Date": "2009-06-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.6200008392334
      },
      {
        "Date": "2009-06-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.770000457763672
      },
      {
        "Date": "2009-06-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.270000457763672
      },
      {
        "Date": "2009-06-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.459999084472656
      },
      {
        "Date": "2009-06-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.110000610351562
      },
      {
        "Date": "2009-06-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.149999618530273
      },
      {
        "Date": "2009-06-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.809999465942383
      },
      {
        "Date": "2009-06-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.68000030517578
      },
      {
        "Date": "2009-06-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.540000915527344
      },
      {
        "Date": "2009-06-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.030000686645508
      },
      {
        "Date": "2009-06-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.989999771118164
      },
      {
        "Date": "2009-06-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.170000076293945
      },
      {
        "Date": "2009-06-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.579999923706055
      },
      {
        "Date": "2009-06-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.049999237060547
      },
      {
        "Date": "2009-06-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.360000610351562
      },
      {
        "Date": "2009-06-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.93000030517578
      },
      {
        "Date": "2009-06-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.350000381469727
      },
      {
        "Date": "2009-06-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.350000381469727
      },
      {
        "Date": "2009-07-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.219999313354492
      },
      {
        "Date": "2009-07-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.950000762939453
      },
      {"Date": "2009-07-06T00:00:00", "Bank": "^VIX", "Stock Price": 29},
      {
        "Date": "2009-07-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.850000381469727
      },
      {
        "Date": "2009-07-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.299999237060547
      },
      {
        "Date": "2009-07-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.780000686645508
      },
      {
        "Date": "2009-07-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.020000457763672
      },
      {
        "Date": "2009-07-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.309999465942383
      },
      {
        "Date": "2009-07-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.020000457763672
      },
      {
        "Date": "2009-07-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.889999389648438
      },
      {
        "Date": "2009-07-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.420000076293945
      },
      {
        "Date": "2009-07-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.34000015258789
      },
      {
        "Date": "2009-07-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.399999618530273
      },
      {
        "Date": "2009-07-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.8700008392334
      },
      {
        "Date": "2009-07-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.469999313354492
      },
      {
        "Date": "2009-07-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.43000030517578
      },
      {
        "Date": "2009-07-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.09000015258789
      },
      {
        "Date": "2009-07-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.280000686645508
      },
      {
        "Date": "2009-07-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.010000228881836
      },
      {
        "Date": "2009-07-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.610000610351562
      },
      {
        "Date": "2009-07-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.399999618530273
      },
      {
        "Date": "2009-07-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.920000076293945
      },
      {
        "Date": "2009-08-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.559999465942383
      },
      {
        "Date": "2009-08-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.889999389648438
      },
      {
        "Date": "2009-08-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.899999618530273
      },
      {
        "Date": "2009-08-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.670000076293945
      },
      {
        "Date": "2009-08-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.760000228881836
      },
      {
        "Date": "2009-08-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.989999771118164
      },
      {
        "Date": "2009-08-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.989999771118164
      },
      {
        "Date": "2009-08-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.450000762939453
      },
      {
        "Date": "2009-08-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.709999084472656
      },
      {
        "Date": "2009-08-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.270000457763672
      },
      {
        "Date": "2009-08-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.889999389648438
      },
      {
        "Date": "2009-08-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.18000030517578
      },
      {
        "Date": "2009-08-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.260000228881836
      },
      {
        "Date": "2009-08-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.09000015258789
      },
      {
        "Date": "2009-08-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.010000228881836
      },
      {
        "Date": "2009-08-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.139999389648438
      },
      {
        "Date": "2009-08-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.920000076293945
      },
      {
        "Date": "2009-08-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.950000762939453
      },
      {
        "Date": "2009-08-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.68000030517578
      },
      {
        "Date": "2009-08-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.760000228881836
      },
      {
        "Date": "2009-08-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.010000228881836
      },
      {
        "Date": "2009-09-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.149999618530273
      },
      {
        "Date": "2009-09-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.899999618530273
      },
      {
        "Date": "2009-09-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.100000381469727
      },
      {
        "Date": "2009-09-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.260000228881836
      },
      {
        "Date": "2009-09-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.6200008392334
      },
      {
        "Date": "2009-09-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.31999969482422
      },
      {
        "Date": "2009-09-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.549999237060547
      },
      {
        "Date": "2009-09-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.149999618530273
      },
      {
        "Date": "2009-09-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.860000610351562
      },
      {
        "Date": "2009-09-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.420000076293945
      },
      {
        "Date": "2009-09-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.690000534057617
      },
      {
        "Date": "2009-09-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.649999618530273
      },
      {
        "Date": "2009-09-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.920000076293945
      },
      {
        "Date": "2009-09-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.059999465942383
      },
      {
        "Date": "2009-09-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.079999923706055
      },
      {
        "Date": "2009-09-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.489999771118164
      },
      {
        "Date": "2009-09-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.950000762939453
      },
      {
        "Date": "2009-09-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.610000610351562
      },
      {
        "Date": "2009-09-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.8799991607666
      },
      {
        "Date": "2009-09-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.190000534057617
      },
      {
        "Date": "2009-09-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.610000610351562
      },
      {
        "Date": "2009-10-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.270000457763672
      },
      {
        "Date": "2009-10-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.68000030517578
      },
      {
        "Date": "2009-10-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.84000015258789
      },
      {
        "Date": "2009-10-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.700000762939453
      },
      {
        "Date": "2009-10-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.68000030517578
      },
      {
        "Date": "2009-10-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.18000030517578
      },
      {
        "Date": "2009-10-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.1200008392334
      },
      {
        "Date": "2009-10-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.010000228881836
      },
      {
        "Date": "2009-10-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.989999771118164
      },
      {
        "Date": "2009-10-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.860000610351562
      },
      {
        "Date": "2009-10-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.719999313354492
      },
      {
        "Date": "2009-10-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.43000030517578
      },
      {
        "Date": "2009-10-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.489999771118164
      },
      {
        "Date": "2009-10-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.899999618530273
      },
      {
        "Date": "2009-10-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.219999313354492
      },
      {
        "Date": "2009-10-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.690000534057617
      },
      {
        "Date": "2009-10-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.270000457763672
      },
      {
        "Date": "2009-10-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.309999465942383
      },
      {
        "Date": "2009-10-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.829999923706055
      },
      {
        "Date": "2009-10-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.90999984741211
      },
      {
        "Date": "2009-10-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.760000228881836
      },
      {
        "Date": "2009-10-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.690000534057617
      },
      {
        "Date": "2009-11-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.780000686645508
      },
      {
        "Date": "2009-11-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.809999465942383
      },
      {
        "Date": "2009-11-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.719999313354492
      },
      {
        "Date": "2009-11-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.43000030517578
      },
      {
        "Date": "2009-11-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.190000534057617
      },
      {
        "Date": "2009-11-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.149999618530273
      },
      {
        "Date": "2009-11-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.84000015258789
      },
      {
        "Date": "2009-11-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.040000915527344
      },
      {
        "Date": "2009-11-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.239999771118164
      },
      {
        "Date": "2009-11-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.360000610351562
      },
      {
        "Date": "2009-11-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.889999389648438
      },
      {
        "Date": "2009-11-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.40999984741211
      },
      {
        "Date": "2009-11-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.6299991607666
      },
      {
        "Date": "2009-11-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.6299991607666
      },
      {
        "Date": "2009-11-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.190000534057617
      },
      {
        "Date": "2009-11-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.15999984741211
      },
      {
        "Date": "2009-11-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.469999313354492
      },
      {
        "Date": "2009-11-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.479999542236328
      },
      {
        "Date": "2009-11-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.739999771118164
      },
      {
        "Date": "2009-11-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.510000228881836
      },
      {
        "Date": "2009-12-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.920000076293945
      },
      {
        "Date": "2009-12-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.1200008392334
      },
      {
        "Date": "2009-12-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.459999084472656
      },
      {"Date": "2009-12-04T00:00:00", "Bank": "^VIX", "Stock Price": 21.25},
      {
        "Date": "2009-12-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.100000381469727
      },
      {
        "Date": "2009-12-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.690000534057617
      },
      {
        "Date": "2009-12-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.65999984741211
      },
      {
        "Date": "2009-12-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.31999969482422
      },
      {
        "Date": "2009-12-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.59000015258789
      },
      {
        "Date": "2009-12-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.149999618530273
      },
      {
        "Date": "2009-12-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.489999771118164
      },
      {
        "Date": "2009-12-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.540000915527344
      },
      {
        "Date": "2009-12-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.510000228881836
      },
      {
        "Date": "2009-12-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.68000030517578
      },
      {
        "Date": "2009-12-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.489999771118164
      },
      {
        "Date": "2009-12-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.540000915527344
      },
      {
        "Date": "2009-12-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.709999084472656
      },
      {
        "Date": "2009-12-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.469999313354492
      },
      {
        "Date": "2009-12-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.93000030517578
      },
      {
        "Date": "2009-12-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.010000228881836
      },
      {
        "Date": "2009-12-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.959999084472656
      },
      {
        "Date": "2009-12-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.68000030517578
      },
      {
        "Date": "2010-01-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.040000915527344
      },
      {
        "Date": "2010-01-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.350000381469727
      },
      {
        "Date": "2010-01-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.15999984741211
      },
      {
        "Date": "2010-01-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.059999465942383
      },
      {
        "Date": "2010-01-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.1299991607666
      },
      {
        "Date": "2010-01-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.549999237060547
      },
      {"Date": "2010-01-12T00:00:00", "Bank": "^VIX", "Stock Price": 18.25},
      {
        "Date": "2010-01-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.850000381469727
      },
      {
        "Date": "2010-01-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.6299991607666
      },
      {
        "Date": "2010-01-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.90999984741211
      },
      {
        "Date": "2010-01-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.579999923706055
      },
      {
        "Date": "2010-01-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.68000030517578
      },
      {
        "Date": "2010-01-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.270000457763672
      },
      {
        "Date": "2010-01-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.309999465942383
      },
      {
        "Date": "2010-01-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.40999984741211
      },
      {
        "Date": "2010-01-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.549999237060547
      },
      {
        "Date": "2010-01-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.139999389648438
      },
      {
        "Date": "2010-01-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.729999542236328
      },
      {
        "Date": "2010-01-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.6200008392334
      },
      {
        "Date": "2010-02-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.59000015258789
      },
      {
        "Date": "2010-02-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.479999542236328
      },
      {
        "Date": "2010-02-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.600000381469727
      },
      {
        "Date": "2010-02-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.079999923706055
      },
      {
        "Date": "2010-02-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.110000610351562
      },
      {
        "Date": "2010-02-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.510000228881836
      },
      {"Date": "2010-02-09T00:00:00", "Bank": "^VIX", "Stock Price": 26},
      {
        "Date": "2010-02-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.399999618530273
      },
      {
        "Date": "2010-02-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.959999084472656
      },
      {
        "Date": "2010-02-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.729999542236328
      },
      {"Date": "2010-02-16T00:00:00", "Bank": "^VIX", "Stock Price": 22.25},
      {
        "Date": "2010-02-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.719999313354492
      },
      {
        "Date": "2010-02-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.6299991607666
      },
      {
        "Date": "2010-02-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.020000457763672
      },
      {
        "Date": "2010-02-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.940000534057617
      },
      {
        "Date": "2010-02-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.3700008392334
      },
      {
        "Date": "2010-02-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.270000457763672
      },
      {
        "Date": "2010-02-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.100000381469727
      },
      {"Date": "2010-02-26T00:00:00", "Bank": "^VIX", "Stock Price": 19.5},
      {
        "Date": "2010-03-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.260000228881836
      },
      {
        "Date": "2010-03-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.059999465942383
      },
      {
        "Date": "2010-03-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.829999923706055
      },
      {
        "Date": "2010-03-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.719999313354492
      },
      {
        "Date": "2010-03-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.420000076293945
      },
      {
        "Date": "2010-03-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.790000915527344
      },
      {
        "Date": "2010-03-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.920000076293945
      },
      {
        "Date": "2010-03-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.56999969482422
      },
      {
        "Date": "2010-03-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.059999465942383
      },
      {
        "Date": "2010-03-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.579999923706055
      },
      {"Date": "2010-03-15T00:00:00", "Bank": "^VIX", "Stock Price": 18},
      {
        "Date": "2010-03-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.690000534057617
      },
      {
        "Date": "2010-03-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.90999984741211
      },
      {
        "Date": "2010-03-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.6200008392334
      },
      {
        "Date": "2010-03-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.969999313354492
      },
      {
        "Date": "2010-03-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.8700008392334
      },
      {
        "Date": "2010-03-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.350000381469727
      },
      {
        "Date": "2010-03-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.549999237060547
      },
      {
        "Date": "2010-03-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.399999618530273
      },
      {
        "Date": "2010-03-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.770000457763672
      },
      {
        "Date": "2010-03-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.59000015258789
      },
      {
        "Date": "2010-03-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.1299991607666
      },
      {
        "Date": "2010-03-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.59000015258789
      },
      {
        "Date": "2010-04-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.469999313354492
      },
      {
        "Date": "2010-04-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.020000457763672
      },
      {
        "Date": "2010-04-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.229999542236328
      },
      {
        "Date": "2010-04-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.6200008392334
      },
      {
        "Date": "2010-04-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.479999542236328
      },
      {
        "Date": "2010-04-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.139999389648438
      },
      {
        "Date": "2010-04-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.579999923706055
      },
      {
        "Date": "2010-04-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.200000762939453
      },
      {
        "Date": "2010-04-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.59000015258789
      },
      {
        "Date": "2010-04-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.890000343322754
      },
      {
        "Date": "2010-04-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.360000610351562
      },
      {
        "Date": "2010-04-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.34000015258789
      },
      {
        "Date": "2010-04-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.729999542236328
      },
      {
        "Date": "2010-04-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.31999969482422
      },
      {
        "Date": "2010-04-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.469999313354492
      },
      {
        "Date": "2010-04-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.6200008392334
      },
      {
        "Date": "2010-04-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.469999313354492
      },
      {
        "Date": "2010-04-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.809999465942383
      },
      {
        "Date": "2010-04-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.079999923706055
      },
      {
        "Date": "2010-04-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.440000534057617
      },
      {
        "Date": "2010-04-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.049999237060547
      },
      {
        "Date": "2010-05-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.190000534057617
      },
      {
        "Date": "2010-05-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.84000015258789
      },
      {
        "Date": "2010-05-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.90999984741211
      },
      {
        "Date": "2010-05-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.79999923706055
      },
      {
        "Date": "2010-05-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 40.95000076293945
      },
      {
        "Date": "2010-05-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.84000015258789
      },
      {
        "Date": "2010-05-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.31999969482422
      },
      {
        "Date": "2010-05-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.520000457763672
      },
      {
        "Date": "2010-05-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.68000030517578
      },
      {
        "Date": "2010-05-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 31.239999771118164
      },
      {
        "Date": "2010-05-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.84000015258789
      },
      {
        "Date": "2010-05-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.54999923706055
      },
      {
        "Date": "2010-05-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.31999969482422
      },
      {
        "Date": "2010-05-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 45.790000915527344
      },
      {
        "Date": "2010-05-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 40.099998474121094
      },
      {
        "Date": "2010-05-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 38.31999969482422
      },
      {
        "Date": "2010-05-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 34.61000061035156
      },
      {
        "Date": "2010-05-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.02000045776367
      },
      {
        "Date": "2010-05-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.68000030517578
      },
      {
        "Date": "2010-05-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.06999969482422
      },
      {
        "Date": "2010-06-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.540000915527344
      },
      {
        "Date": "2010-06-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.170000076293945
      },
      {
        "Date": "2010-06-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.459999084472656
      },
      {
        "Date": "2010-06-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 35.47999954223633
      },
      {
        "Date": "2010-06-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 36.56999969482422
      },
      {
        "Date": "2010-06-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.70000076293945
      },
      {
        "Date": "2010-06-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 33.72999954223633
      },
      {
        "Date": "2010-06-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.56999969482422
      },
      {
        "Date": "2010-06-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.790000915527344
      },
      {
        "Date": "2010-06-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.579999923706055
      },
      {
        "Date": "2010-06-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.8700008392334
      },
      {
        "Date": "2010-06-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.920000076293945
      },
      {
        "Date": "2010-06-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.049999237060547
      },
      {
        "Date": "2010-06-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.950000762939453
      },
      {
        "Date": "2010-06-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.8799991607666
      },
      {
        "Date": "2010-06-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.049999237060547
      },
      {
        "Date": "2010-06-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.90999984741211
      },
      {
        "Date": "2010-06-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.739999771118164
      },
      {
        "Date": "2010-06-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 28.530000686645508
      },
      {"Date": "2010-06-28T00:00:00", "Bank": "^VIX", "Stock Price": 29},
      {
        "Date": "2010-06-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 34.130001068115234
      },
      {
        "Date": "2010-06-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 34.540000915527344
      },
      {
        "Date": "2010-07-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 32.86000061035156
      },
      {
        "Date": "2010-07-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 30.1200008392334
      },
      {
        "Date": "2010-07-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 29.649999618530273
      },
      {
        "Date": "2010-07-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.84000015258789
      },
      {
        "Date": "2010-07-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.709999084472656
      },
      {
        "Date": "2010-07-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.979999542236328
      },
      {
        "Date": "2010-07-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.43000030517578
      },
      {
        "Date": "2010-07-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.559999465942383
      },
      {
        "Date": "2010-07-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.889999389648438
      },
      {
        "Date": "2010-07-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.139999389648438
      },
      {"Date": "2010-07-16T00:00:00", "Bank": "^VIX", "Stock Price": 26.25},
      {
        "Date": "2010-07-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.969999313354492
      },
      {
        "Date": "2010-07-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.93000030517578
      },
      {
        "Date": "2010-07-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.639999389648438
      },
      {
        "Date": "2010-07-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.6299991607666
      },
      {
        "Date": "2010-07-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.469999313354492
      },
      {
        "Date": "2010-07-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.729999542236328
      },
      {
        "Date": "2010-07-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.190000534057617
      },
      {"Date": "2010-07-28T00:00:00", "Bank": "^VIX", "Stock Price": 24.25},
      {
        "Date": "2010-07-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.1299991607666
      },
      {"Date": "2010-07-30T00:00:00", "Bank": "^VIX", "Stock Price": 23.5},
      {
        "Date": "2010-08-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.010000228881836
      },
      {
        "Date": "2010-08-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.6299991607666
      },
      {
        "Date": "2010-08-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.209999084472656
      },
      {
        "Date": "2010-08-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.100000381469727
      },
      {
        "Date": "2010-08-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.739999771118164
      },
      {
        "Date": "2010-08-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.139999389648438
      },
      {
        "Date": "2010-08-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.3700008392334
      },
      {
        "Date": "2010-08-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.389999389648438
      },
      {
        "Date": "2010-08-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.729999542236328
      },
      {
        "Date": "2010-08-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.239999771118164
      },
      {
        "Date": "2010-08-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.100000381469727
      },
      {
        "Date": "2010-08-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.329999923706055
      },
      {
        "Date": "2010-08-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.59000015258789
      },
      {
        "Date": "2010-08-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.440000534057617
      },
      {
        "Date": "2010-08-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.489999771118164
      },
      {
        "Date": "2010-08-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 25.65999984741211
      },
      {
        "Date": "2010-08-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.459999084472656
      },
      {
        "Date": "2010-08-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.700000762939453
      },
      {
        "Date": "2010-08-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.3700008392334
      },
      {
        "Date": "2010-08-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 24.450000762939453
      },
      {
        "Date": "2010-08-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 27.209999084472656
      },
      {
        "Date": "2010-08-31T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 26.049999237060547
      },
      {
        "Date": "2010-09-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.889999389648438
      },
      {
        "Date": "2010-09-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.190000534057617
      },
      {
        "Date": "2010-09-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.309999465942383
      },
      {
        "Date": "2010-09-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.799999237060547
      },
      {"Date": "2010-09-08T00:00:00", "Bank": "^VIX", "Stock Price": 23.25},
      {
        "Date": "2010-09-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.809999465942383
      },
      {
        "Date": "2010-09-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.989999771118164
      },
      {
        "Date": "2010-09-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.209999084472656
      },
      {
        "Date": "2010-09-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.559999465942383
      },
      {
        "Date": "2010-09-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.100000381469727
      },
      {
        "Date": "2010-09-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.719999313354492
      },
      {
        "Date": "2010-09-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.010000228881836
      },
      {"Date": "2010-09-20T00:00:00", "Bank": "^VIX", "Stock Price": 21.5},
      {
        "Date": "2010-09-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.350000381469727
      },
      {
        "Date": "2010-09-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.510000228881836
      },
      {
        "Date": "2010-09-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.8700008392334
      },
      {
        "Date": "2010-09-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.709999084472656
      },
      {
        "Date": "2010-09-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.540000915527344
      },
      {
        "Date": "2010-09-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.600000381469727
      },
      {"Date": "2010-09-29T00:00:00", "Bank": "^VIX", "Stock Price": 23.25},
      {
        "Date": "2010-09-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.700000762939453
      },
      {"Date": "2010-10-01T00:00:00", "Bank": "^VIX", "Stock Price": 22.5},
      {
        "Date": "2010-10-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.530000686645508
      },
      {
        "Date": "2010-10-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.760000228881836
      },
      {
        "Date": "2010-10-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.489999771118164
      },
      {
        "Date": "2010-10-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.559999465942383
      },
      {
        "Date": "2010-10-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.709999084472656
      },
      {
        "Date": "2010-10-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.959999084472656
      },
      {
        "Date": "2010-10-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.93000030517578
      },
      {
        "Date": "2010-10-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.06999969482422
      },
      {
        "Date": "2010-10-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.8799991607666
      },
      {
        "Date": "2010-10-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.030000686645508
      },
      {
        "Date": "2010-10-18T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.09000015258789
      },
      {
        "Date": "2010-10-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.6299991607666
      },
      {
        "Date": "2010-10-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.790000915527344
      },
      {
        "Date": "2010-10-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.270000457763672
      },
      {
        "Date": "2010-10-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.780000686645508
      },
      {
        "Date": "2010-10-25T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.850000381469727
      },
      {
        "Date": "2010-10-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.219999313354492
      },
      {
        "Date": "2010-10-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.709999084472656
      },
      {
        "Date": "2010-10-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.8799991607666
      },
      {
        "Date": "2010-10-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.200000762939453
      },
      {
        "Date": "2010-11-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.829999923706055
      },
      {
        "Date": "2010-11-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.56999969482422
      },
      {
        "Date": "2010-11-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.559999465942383
      },
      {
        "Date": "2010-11-04T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.520000457763672
      },
      {
        "Date": "2010-11-05T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.260000228881836
      },
      {
        "Date": "2010-11-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.290000915527344
      },
      {
        "Date": "2010-11-09T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.079999923706055
      },
      {
        "Date": "2010-11-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.469999313354492
      },
      {
        "Date": "2010-11-11T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.639999389648438
      },
      {
        "Date": "2010-11-12T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.610000610351562
      },
      {
        "Date": "2010-11-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.200000762939453
      },
      {
        "Date": "2010-11-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.579999923706055
      },
      {
        "Date": "2010-11-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.760000228881836
      },
      {"Date": "2010-11-18T00:00:00", "Bank": "^VIX", "Stock Price": 18.75},
      {
        "Date": "2010-11-19T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.040000915527344
      },
      {
        "Date": "2010-11-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.3700008392334
      },
      {
        "Date": "2010-11-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 20.6299991607666
      },
      {
        "Date": "2010-11-24T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.559999465942383
      },
      {
        "Date": "2010-11-26T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 22.219999313354492
      },
      {
        "Date": "2010-11-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.530000686645508
      },
      {
        "Date": "2010-11-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 23.540000915527344
      },
      {
        "Date": "2010-12-01T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 21.360000610351562
      },
      {
        "Date": "2010-12-02T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 19.389999389648438
      },
      {
        "Date": "2010-12-03T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.010000228881836
      },
      {
        "Date": "2010-12-06T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 18.020000457763672
      },
      {
        "Date": "2010-12-07T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.989999771118164
      },
      {
        "Date": "2010-12-08T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.739999771118164
      },
      {"Date": "2010-12-09T00:00:00", "Bank": "^VIX", "Stock Price": 17.25},
      {
        "Date": "2010-12-10T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.610000610351562
      },
      {
        "Date": "2010-12-13T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.549999237060547
      },
      {
        "Date": "2010-12-14T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.610000610351562
      },
      {
        "Date": "2010-12-15T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.940000534057617
      },
      {
        "Date": "2010-12-16T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.389999389648438
      },
      {
        "Date": "2010-12-17T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.110000610351562
      },
      {
        "Date": "2010-12-20T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.40999984741211
      },
      {
        "Date": "2010-12-21T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.489999771118164
      },
      {
        "Date": "2010-12-22T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 15.449999809265137
      },
      {
        "Date": "2010-12-23T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 16.469999313354492
      },
      {
        "Date": "2010-12-27T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.670000076293945
      },
      {
        "Date": "2010-12-28T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.520000457763672
      },
      {
        "Date": "2010-12-29T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.280000686645508
      },
      {
        "Date": "2010-12-30T00:00:00",
        "Bank": "^VIX",
        "Stock Price": 17.520000457763672
      }
    ]
  }
};
    vegaEmbed("#vis", spec, {mode: "vega-lite"}).then(console.log).catch(console.warn);
  </script>
</body>
</html>

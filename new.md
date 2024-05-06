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
      "data": {"name": "data-f5aed9d134fc5f5a2956b854f12b0cea"},
      "mark": {"type": "circle", "color": "orange"},
      "encoding": {
        "tooltip": [
          {
            "field": "FPCPITOTLZGUSA",
            "title": "Inflation",
            "type": "quantitative"
          }
        ],
        "x": {"field": "DATE", "type": "temporal"},
        "y": {"axis": null, "field": "FPCPITOTLZGUSA", "type": "quantitative"}
      }
    },
    {
      "data": {"name": "data-440d6f07ec99fcb97167acbeb25d32be"},
      "mark": {"type": "circle", "color": "orange"},
      "encoding": {
        "tooltip": [
          {"field": "MEDCPIM158SFRBCLE", "title": "CPI", "type": "quantitative"}
        ],
        "x": {"field": "DATE", "type": "temporal"},
        "y": {
          "axis": null,
          "field": "MEDCPIM158SFRBCLE",
          "type": "quantitative"
        }
      }
    },
    {
      "data": {"name": "data-f5aed9d134fc5f5a2956b854f12b0cea"},
      "mark": {"type": "line", "color": "blue", "interpolate": "monotone"},
      "encoding": {
        "x": {"field": "DATE", "type": "temporal"},
        "y": {
          "field": "FPCPITOTLZGUSA",
          "title": "Inflation (%)",
          "type": "quantitative"
        }
      }
    },
    {
      "data": {"name": "data-440d6f07ec99fcb97167acbeb25d32be"},
      "mark": {"type": "line", "color": "teal", "interpolate": "monotone"},
      "encoding": {
        "x": {"field": "DATE", "type": "temporal"},
        "y": {
          "field": "MEDCPIM158SFRBCLE",
          "title": "CPI",
          "type": "quantitative"
        }
      }
    }
  ],
  "height": 500,
  "resolve": {"scale": {"y": "independent"}},
  "title": "Inflation Rate vs. CPI (2005 - 2010)",
  "width": 700,
  "$schema": "https://vega.github.io/schema/vega-lite/v4.17.0.json",
  "datasets": {
    "data-f5aed9d134fc5f5a2956b854f12b0cea": [
      {"DATE": "2005-01-01", "FPCPITOTLZGUSA": 3.3927468454955},
      {"DATE": "2006-01-01", "FPCPITOTLZGUSA": 3.22594410070404},
      {"DATE": "2007-01-01", "FPCPITOTLZGUSA": 2.85267248150138},
      {"DATE": "2008-01-01", "FPCPITOTLZGUSA": 3.839100296651},
      {"DATE": "2009-01-01", "FPCPITOTLZGUSA": -0.355546266299747},
      {"DATE": "2010-01-01", "FPCPITOTLZGUSA": 1.6400434423899}
    ],
    "data-440d6f07ec99fcb97167acbeb25d32be": [
      {"DATE": "2005-01-01", "MEDCPIM158SFRBCLE": 3.4217591363454103},
      {"DATE": "2005-02-01", "MEDCPIM158SFRBCLE": 3.30400229074104},
      {"DATE": "2005-03-01", "MEDCPIM158SFRBCLE": 1.8971793950121696},
      {"DATE": "2005-04-01", "MEDCPIM158SFRBCLE": 2.09647901335652},
      {"DATE": "2005-05-01", "MEDCPIM158SFRBCLE": 3.16846235161856},
      {"DATE": "2005-06-01", "MEDCPIM158SFRBCLE": 1.62477538920178},
      {"DATE": "2005-07-01", "MEDCPIM158SFRBCLE": 3.0286455734746403},
      {"DATE": "2005-08-01", "MEDCPIM158SFRBCLE": 2.22215620270876},
      {"DATE": "2005-09-01", "MEDCPIM158SFRBCLE": 4.02470724061161},
      {"DATE": "2005-10-01", "MEDCPIM158SFRBCLE": 3.3315751559861897},
      {"DATE": "2005-11-01", "MEDCPIM158SFRBCLE": 2.83691194814226},
      {"DATE": "2005-12-01", "MEDCPIM158SFRBCLE": 2.20489319920401},
      {"DATE": "2006-01-01", "MEDCPIM158SFRBCLE": 2.88432186623886},
      {"DATE": "2006-02-01", "MEDCPIM158SFRBCLE": 2.07202087371556},
      {"DATE": "2006-03-01", "MEDCPIM158SFRBCLE": 3.08218251360963},
      {"DATE": "2006-04-01", "MEDCPIM158SFRBCLE": 2.8870316165126},
      {"DATE": "2006-05-01", "MEDCPIM158SFRBCLE": 4.28816068458393},
      {"DATE": "2006-06-01", "MEDCPIM158SFRBCLE": 3.19983083499134},
      {"DATE": "2006-07-01", "MEDCPIM158SFRBCLE": 3.05393052415284},
      {"DATE": "2006-08-01", "MEDCPIM158SFRBCLE": 4.62137039677921},
      {"DATE": "2006-09-01", "MEDCPIM158SFRBCLE": 2.1062637733366696},
      {"DATE": "2006-10-01", "MEDCPIM158SFRBCLE": 3.6506970400157694},
      {"DATE": "2006-11-01", "MEDCPIM158SFRBCLE": 3.02469916751935},
      {"DATE": "2006-12-01", "MEDCPIM158SFRBCLE": 2.72554654380133},
      {"DATE": "2007-01-01", "MEDCPIM158SFRBCLE": 2.9644102631689195},
      {"DATE": "2007-02-01", "MEDCPIM158SFRBCLE": 4.4470256400193495},
      {"DATE": "2007-03-01", "MEDCPIM158SFRBCLE": 2.6885311218425296},
      {"DATE": "2007-04-01", "MEDCPIM158SFRBCLE": 2.36832536836802},
      {"DATE": "2007-05-01", "MEDCPIM158SFRBCLE": 2.35349143799752},
      {"DATE": "2007-06-01", "MEDCPIM158SFRBCLE": 3.2680317367730405},
      {"DATE": "2007-07-01", "MEDCPIM158SFRBCLE": 2.82817098511783},
      {"DATE": "2007-08-01", "MEDCPIM158SFRBCLE": 2.18457280462696},
      {"DATE": "2007-09-01", "MEDCPIM158SFRBCLE": 3.7044060077008303},
      {"DATE": "2007-10-01", "MEDCPIM158SFRBCLE": 3.43463052089827},
      {"DATE": "2007-11-01", "MEDCPIM158SFRBCLE": 3.475359352757},
      {"DATE": "2007-12-01", "MEDCPIM158SFRBCLE": 2.98265388398264},
      {"DATE": "2008-01-01", "MEDCPIM158SFRBCLE": 3.28360527628442},
      {"DATE": "2008-02-01", "MEDCPIM158SFRBCLE": 2.85747436326564},
      {"DATE": "2008-03-01", "MEDCPIM158SFRBCLE": 3.0404857461239905},
      {"DATE": "2008-04-01", "MEDCPIM158SFRBCLE": 2.24101388446512},
      {"DATE": "2008-05-01", "MEDCPIM158SFRBCLE": 2.4627692895931},
      {"DATE": "2008-06-01", "MEDCPIM158SFRBCLE": 4.05370089545272},
      {"DATE": "2008-07-01", "MEDCPIM158SFRBCLE": 3.98912873927892},
      {"DATE": "2008-08-01", "MEDCPIM158SFRBCLE": 2.94013128490127},
      {"DATE": "2008-09-01", "MEDCPIM158SFRBCLE": 3.17438970761372},
      {"DATE": "2008-10-01", "MEDCPIM158SFRBCLE": 2.20171024216991},
      {"DATE": "2008-11-01", "MEDCPIM158SFRBCLE": 1.93625366578525},
      {"DATE": "2008-12-01", "MEDCPIM158SFRBCLE": 0.3634841508005421},
      {"DATE": "2009-01-01", "MEDCPIM158SFRBCLE": 2.40364062502632},
      {"DATE": "2009-02-01", "MEDCPIM158SFRBCLE": 2.14357605719473},
      {"DATE": "2009-03-01", "MEDCPIM158SFRBCLE": 1.90828983085518},
      {"DATE": "2009-04-01", "MEDCPIM158SFRBCLE": 1.86117019943739},
      {"DATE": "2009-05-01", "MEDCPIM158SFRBCLE": 1.29376893720741},
      {"DATE": "2009-06-01", "MEDCPIM158SFRBCLE": 0.75584590889346},
      {"DATE": "2009-07-01", "MEDCPIM158SFRBCLE": 0.125832513392354},
      {"DATE": "2009-08-01", "MEDCPIM158SFRBCLE": 1.6255061079099},
      {"DATE": "2009-09-01", "MEDCPIM158SFRBCLE": 0.914369783533586},
      {"DATE": "2009-10-01", "MEDCPIM158SFRBCLE": 1.1903654188135},
      {"DATE": "2009-11-01", "MEDCPIM158SFRBCLE": 0.516016421313492},
      {"DATE": "2009-12-01", "MEDCPIM158SFRBCLE": 0.460810409841406},
      {"DATE": "2010-01-01", "MEDCPIM158SFRBCLE": 0.680110845940707},
      {"DATE": "2010-02-01", "MEDCPIM158SFRBCLE": -0.1066278542679489},
      {"DATE": "2010-03-01", "MEDCPIM158SFRBCLE": -0.286064246298046}
    ]
  }
};
    vegaEmbed("#vis", spec, {mode: "vega-lite"}).then(console.log).catch(console.warn);
  </script>
</body>
</html>

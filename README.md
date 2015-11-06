-----

[![build status](https://api.travis-ci.org/litaotao/IPython-Dashboard.svg?branch=v-0.2-dashboard-server)](https://travis-ci.org/litaotao/IPython-Dashboard)  [![coverage](https://coveralls.io/repos/litaotao/IPython-Dashboard/badge.svg?branch=v-0.2-dashboard-server&service=github)](https://coveralls.io/r/litaotao/IPython-Dashboard)  [![Documentation Status](https://readthedocs.org/projects/ipython-dashboard/badge/?version=latest)](http://ipython-dashboard.readthedocs.org/en/latest/?badge=latest)   [![PyPI Version](http://img.shields.io/pypi/v/IPython-Dashboard.svg)](https://pypi.python.org/pypi/IPython-Dashboard)


-----

## ***Inspired by [IPython](http://ipython.org/), built for data guy***

-----

# IPython-Dashboard
A stand alone, light-weight web server for building, sharing graphs created in ipython. Build for data science, data analysis guys. Building an interactive visualization, collaborated dashboard, and real-time streaming graph.

-----

# Goal

- support raw html visualization
- support python object visualization
- Editable
- Real-time fresh when rendering a variable python object
- Can be shared, both public and private [ need password ]
- In the notebook, can share an object to a dashboard [ that's visualise that object in that dashboard ]

-----

# Screenshot and Demo

[Demo on Youtube](https://youtu.be/Xv0UjKVEttA)     
[Demo on Youku](http://v.youku.com/v_show/id_XMTM3MTc5MTAwMA)

[![demo](docs/template-screenshot-1.jpg)](https://youtu.be/Xv0UjKVEttA)
[![demo](docs/template-screenshot-2.jpg)](https://youtu.be/Xv0UjKVEttA)
[![demo](docs/template-screenshot-3.jpg)](https://youtu.be/Xv0UjKVEttA)

-----


# Usage
![docs/usage-1.jpg](docs/usage-1.jpg)

-----


# Run tests

just run `sudo nosetests --with-coverage --cover-package=dashboard` under this repo

```
aaron@aarons-MacBook-Pro:~/Desktop/github/IPython-Dashboard$sudo nosetests --with-coverage --cover-package=dashboard
...
Name                                    Stmts   Miss  Cover   Missing
---------------------------------------------------------------------
dashboard.py                                9      0   100%
dashboard/client.py                         1      0   100%
dashboard/client/sender.py                 11      9    18%   22-34
dashboard/config.py                        12      0   100%
dashboard/server.py                         1      0   100%
dashboard/server/resources.py               0      0   100%
dashboard/server/resources/dash.py         41     25    39%   25-30, 39, 48-49, 55-71, 76-87
dashboard/server/resources/home.py          8      1    88%   20
dashboard/server/resources/storage.py      15      7    53%   20-22, 30-34
dashboard/server/utils.py                  31      6    81%   18-22, 29, 43
dashboard/server/views.py                  12      0   100%
---------------------------------------------------------------------
TOTAL                                     141     48    66%
----------------------------------------------------------------------
Ran 3 tests in 0.345s

OK
```

-----

# Change Log



- future
    + import dashboard to ipython notebook, one click [ though I don't think it's necessary]
    + front side, databricks style
    + pep 8, code clean up & restructure
    + hover tips
    + edit modal can be resized
    + Share one graph
    + Share one dashboard
    + Presentation mode
    + slogan
    + footer
    + readthedoc
    + unified message display center
    + SQL Editor
    + login management
    + unified logger and exception report




- ***V 0.1.2 : visualiza-table : [ current develop version ]***
    - slogan: ***Inspired by IPython, built for data guy***

    - Dashboard
        + document and doc string
        + usage
        + simple visualize table data

    - SQL Editor
        + research & preparation


- ***V 0.1.1 : dashboard-server : [ current stable release ]***  
    - Dashboard
        - dashboard home page
            + sort by dashboard name / creator / last update time

        - dashboard page
            + add graph in a dashboard
            + re-arrange graph
            + resize graph
            + get table view in a graph

    - SQL Editor



- V 0.1 : dashboard-template
    + Add dashboard client template
    + Template consists of box, each box is an independent front-side object
    + Template hierarchy:
        + box page [add, delete, share one or all]
        + box graph [add, delete, share one or all]
        + rename

-----


# Related Projects & Products

- [mpld3](https://github.com/jakevdp/mpld3)
- [lighting](http://lightning-viz.org/)
- [bokeh](http://bokeh.pydata.org/en/latest/)
- [matplotlib](http://matplotlib.org)
- [zeppelin](https://github.com/apache/incubator-zeppelin)
- [yhat](https://github.com/yhat/rodeo)
- [hue](https://github.com/cloudera/hue)
- [plotly](https://github.com/plotly/dashboards)
- [datadog](https://www.datadoghq.com)
- [databricks](https://databricks.com/)
- [nvd3](http://nvd3.org/)
- [c3js](http://c3js.org/)
- [periscope](http://periscope.io)
- [folium](https://github.com/python-visualization/folium)
- [metabase](http://www.metabase.com/)
- [gridstack](https://github.com/troolee/gridstack.js)
- [gridster](http://gridster.net/)

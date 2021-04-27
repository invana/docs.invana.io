# Installing Invana Engine

## Installing using Docker

```
$ docker run -p 8200:8200 -d  -e GREMLIN_SERVER_URL=ws://xx.xx.xx.xx:8182/gremlin --name invana-engine invanalabs/invana-engine 
```

<table>
  <thead>
    <tr>
      <th style="text-align:left">Environment variable name</th>
      <th style="text-align:left">optional</th>
      <th style="text-align:left">default</th>
      <th style="text-align:left">description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li><b>GREMLIN_SERVER_URL</b>
          </li>
        </ul>
      </td>
      <td style="text-align:left">false</td>
      <td style="text-align:left">None</td>
      <td style="text-align:left">
        <p></p>
        <ul>
          <li>http or ws gremlin url. ex: ws://xx.xx.xx.xx:8182/gremlin or <a href="http://xx.xx.xx.xx:8182/gremlin">http://xx.xx.xx.xx:8182/gremlin</a>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

* **GREMLIN\_SERVER\_URL**: http or ws gremlin url. ex: ws://xx.xx.xx.xx:8182/gremlin or [http://xx.xx.xx.xx:8182/gremlin](http://xx.xx.xx.xx:8182/gremlin)
* **GREMLIN\_TRAVERSAL\_SOURCE**\(optional\): defaults: 'g'
* **GREMLIN\_SERVER\_USERNAME**\(optional\): gremlin username. ex: myusername
* **GREMLIN\_SERVER\_PASSWORD**\(optional\): gremlin password. ex: mypassword
* **SERVER\_PORT**\(optional, available in standalone python mode only\): port on which invana engine server is available: defaults to 8200


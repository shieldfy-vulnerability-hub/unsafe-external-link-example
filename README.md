# unsafe-external-link-example

## there is 3 vulnerabilities

1. unsafe_external_link in `ejs.vuln.ejs` line `27`

```ejs
      </li>
      <% } %>
      <li class="nav-item">
        <a class="nav-link" href="<%= url %>" target="_blank">About</a>
      </li>
    </ul>
  </div>
```

2. unsafe_external_link in `hbs.vuln.hbs` line `10`

```hbs
<title>Document</title>
</head>
<body>
    <a href="{{url}}" target="_blank">Visit Shieldfy</a>
</body>
</html>

```

3. unsafe_external_link in `mustache.vuln.html` line `10`

```html
<title>Document</title>
</head>
<body>
    <a href="{{ url }}" target="_blank">Visit Shieldfy</a>
</body>
</html>
```

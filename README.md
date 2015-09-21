#### Variety of snippets

##### List all module dependencies sorted with versions
This is good to find duplication. I had to work with this when
I had a conflict in passport version references between passport 0.3.0
and passport 0.2.0 which is used by password-google-openidconnect.

```javascript
    npm ls | sed -E 's/(.+) (.+)$/\2/' | sort
```


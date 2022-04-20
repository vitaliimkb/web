# This is my repository

### My name is Vitalii

![My photo](https://i.ytimg.com/vi/1Ne1hqOXKKI/maxresdefault.jpg)

**I'm java script developer**
*There is example of my code*
```python
$('input').on('change', function () {
    let username = $('input').val()
    $.ajax(`https://api.github.com/users/${username}`, {
        success: function(result) {
            $("#result").html(`
                <h2>${result.login}</h2>
                <img src='${result.avatar_url}'>
                <a href='${result.html_url}' target="_blank">
                    To profile
                </a>
            `)
        }
    })
})
```

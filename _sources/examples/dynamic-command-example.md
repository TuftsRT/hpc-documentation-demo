# Dynamic Command Example

Tufts Username: <input type="text" id="utln" value="" size="10"> <button onclick="replaceUsername()">OK</button>

```bash
ssh YOUR_UTLN@login.pax.tufts.edu
```
The document itself was still originally written in Markdown with the textbox
and button added as HTML elements. The code performing the replacement can be
embedded into the Markdown document or loaded from a static JavaScript file.

```{note}
This is just some hastily put together JavaScript so it will only work once.
```


<script>
function replaceUsername()
{
    new_username = document.getElementById("utln").value;
    document.body.innerHTML = document.body.innerHTML.replace("YOUR_UTLN", new_username);
}
</script>

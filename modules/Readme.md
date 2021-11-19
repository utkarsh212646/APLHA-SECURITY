## Alpha Example plugin format
```python3
from Alphax.decorator import register
from .utils.disable import disableable_dec
from .utils.message import get_args_str

@register(cmds="Alphax")
@disableable_dec("Alphax")
async def _(message):
    j = "Hello there my name is Alphax"
    await message.reply(j)
    

__help__ = """
<b>Hi</b>
- /hi: Hello there my name is Alphax
"""
__mod_name__ = "Alphax"
```

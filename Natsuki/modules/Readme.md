## wonderwoman Example plugin format
```python3
from wonderwoman.decorator import register
from .utils.disable import disableable_dec
from .utils.message import get_args_str

@register(cmds="wonderwoman")
@disableable_dec("wonderwoman")
async def _(message):
    j = "Hello there my name is wonderwoman"
    await message.reply(j)
    

__help__ = """
<b>Hi</b>
- /hi: Hello there my name is Natsuki
"""
__mod_name__ = "wonderwoman"
```

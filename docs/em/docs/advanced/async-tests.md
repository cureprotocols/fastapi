# 🔁 💯

👆 ✔️ ⏪ 👀 ❔ 💯 👆 **FastAPI** 🈸 ⚙️ 🚚 `TestClient`. 🆙 🔜, 👆 ✔️ 🕴 👀 ❔ ✍ 🔁 💯, 🍵 ⚙️ `async` 🔢.

➖ 💪 ⚙️ 🔁 🔢 👆 💯 💪 ⚠, 🖼, 🕐❔ 👆 🔬 👆 💽 🔁. 🌈 👆 💚 💯 📨 📨 👆 FastAPI 🈸 &amp; ⤴️ ✔ 👈 👆 👩‍💻 ⏪ ✍ ☑ 💽 💽, ⏪ ⚙️ 🔁 💽 🗃.

➡️ 👀 ❔ 👥 💪 ⚒ 👈 👷.

## pytest.mark.anyio

🚥 👥 💚 🤙 🔁 🔢 👆 💯, 👆 💯 🔢 ✔️ 🔁. AnyIO 🚚 👌 📁 👉, 👈 ✔ 👥 ✔ 👈 💯 🔢 🤙 🔁.

## 🇸🇲

🚥 👆 **FastAPI** 🈸 ⚙️ 😐 `def` 🔢 ↩️ `async def`, ⚫️ `async` 🈸 🔘.

`TestClient` 🔨 🎱 🔘 🤙 🔁 FastAPI 🈸 👆 😐 `def` 💯 🔢, ⚙️ 🐩 ✳. ✋️ 👈 🎱 🚫 👷 🚫🔜 🕐❔ 👥 ⚙️ ⚫️ 🔘 🔁 🔢. 🏃 👆 💯 🔁, 👥 💪 🙅‍♂ 📏 ⚙️ `TestClient` 🔘 👆 💯 🔢.

`TestClient` ⚓️ 🔛 <a href="https://www.python-httpx.org" class="external-link" target="_blank">🇸🇲</a>, &amp; ↩️, 👥 💪 ⚙️ ⚫️ 🔗 💯 🛠️.

## 🖼

🙅 🖼, ➡️ 🤔 📁 📊 🎏 1️⃣ 🔬 [🦏 🈸](../tutorial/bigger-applications.md){.internal-link target=_blank} &amp; [🔬](../tutorial/testing.md){.internal-link target=_blank}:

```
.
├── app
│   ├── __init__.py
│   ├── main.py
│   └── test_main.py
```

📁 `main.py` 🔜 ✔️:

{* ../../docs_src/async_tests/main.py *}

📁 `test_main.py` 🔜 ✔️ 💯 `main.py`, ⚫️ 💪 👀 💖 👉 🔜:

{* ../../docs_src/async_tests/test_main.py *}

## 🏃 ⚫️

👆 💪 🏃 👆 💯 🐌 📨:

<div class="termy">

```console
$ pytest

---> 100%
```

</div>

## ℹ

📑 `@pytest.mark.anyio` 💬 ✳ 👈 👉 💯 🔢 🔜 🤙 🔁:

{* ../../docs_src/async_tests/test_main.py hl[7] *}

/// tip

🗒 👈 💯 🔢 🔜 `async def` ↩️ `def` ⏭ 🕐❔ ⚙️ `TestClient`.

///

⤴️ 👥 💪 ✍ `AsyncClient` ⏮️ 📱, &amp; 📨 🔁 📨 ⚫️, ⚙️ `await`.

{* ../../docs_src/async_tests/test_main.py hl[9:12] *}

👉 🌓:

```Python
response = client.get('/')
```

...👈 👥 ⚙️ ⚒ 👆 📨 ⏮️ `TestClient`.

/// tip

🗒 👈 👥 ⚙️ 🔁/⌛ ⏮️ 🆕 `AsyncClient` - 📨 🔁.

///

## 🎏 🔁 🔢 🤙

🔬 🔢 🔜 🔁, 👆 💪 🔜 🤙 (&amp; `await`) 🎏 `async` 🔢 ↖️ ⚪️➡️ 📨 📨 👆 FastAPI 🈸 👆 💯, ⚫️❔ 👆 🔜 🤙 👫 🙆 🙆 👆 📟.

/// tip

🚥 👆 ⚔ `RuntimeError: Task attached to a different loop` 🕐❔ 🛠️ 🔁 🔢 🤙 👆 💯 (✅ 🕐❔ ⚙️ <a href="https://stackoverflow.com/questions/41584243/runtimeerror-task-attached-to-a-different-loop" class="external-link" target="_blank">✳ MotorClient</a>) 💭 🔗 🎚 👈 💪 🎉 ➰ 🕴 🏞 🔁 🔢, ✅ `'@app.on_event("startup")` ⏲.

///

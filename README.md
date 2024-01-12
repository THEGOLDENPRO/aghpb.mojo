<div align="center">

  # 🔥 aghpb.mojo 📚
  <sub>Mojo API wrapper for the anime girls holding programming books [API](https://api.devgoldy.xyz/aghpb/v1/docs)</sub>

</div>

<div align="center">

  <img src="./assets/book_1.png" width="600px">

</div>

<br>

> [!Note]
> 
> This is part of my [aghpb api](https://github.com/THEGOLDENPRO/aghpb_api) wrapper challenge where I attempt to write an api wrapper in every language possible. So yes expect spaghetti code as it will be my first time writing in these languages. Although I'm 100% open to improvements and corrections so feel free to contribute anything.
> **[Other languages I've done](https://github.com/THEGOLDENPRO/aghpb_api#-api-wrappers)**

> [!Warning]
> 
> This is BROKEN and INCOMPLETE because **THIS LANGUAGE IS INCOMPLETE!!!** 😡💢

## Install
idk, this is fucking mojo. It hasn't even been released yet.

so read their docs and find out yourself if you're so nerdy: https://docs.modular.com/mojo/manual/packages.html

## Examples
This is how you may retrieve a random anime girls holding programming books:
```mojo
from python import Python

from aghpb import Client

fn main() raises:
    let python = Python.import_module("builtins")

    let client = Client()
    let book = client.random()

    print(book.name)
    print(book.category)
    print(book.date_added)

    # We have to use python's file open function as mojo's variant is just not working correctly for me.
    let file = python.open("./anime_girl.png", "wb")
    _ = file.write(book.image_bytes)
    _ = file.close()

    # This is how we would have done it in mojo if it wasn't so bad rn.

    # var file = open("./anime_girl.png", "wb")
    # file.write(book.image_bytes)
    # file.close()
```
and yes categories don't fucking work because OF THIS DUMB.... 😠 *alright let's take a chill pill* 

<br>

Made using my API at 👉 https://api.devgoldy.xyz/aghpb/v1/
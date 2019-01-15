<section >
    <div class="grid-wrapper">
        <div class="content">
            ## Getting nbdime
Normally you'd add it via pip :
```
$ pip install nbdime
```
( <strong> we've done this for you already </strong>)
{:.strong}

You get:
- Command line diffing and merging tools
- Web client based tools (offline use)
- Integration with git

        </div>
    </div>
</section>




## Now let's play with this
You should have the contents of our workshop repository in the home directory of your Docker container

<p class= "fragment grow"> [https://github.com/trallard/JNB_reproducible](https://github.com/trallard/JNB_reproducible)
</p>



## Getting started
The most basic example...
diffing two notebooks:
```bash
$ nbdiff -som diff_ex/RNA-sequencing.ipynb diff_ex/RNA-sequencing2.ipynb
```
You can specify the parts to be compared:
- `--sources` / `-s`
- `--outputs`/ `-o`
- `--metadata` / `-m`
- `--attachments` / `-a`
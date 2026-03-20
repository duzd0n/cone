<!DOCTYPE html>
<style>
	body {
    	background-image: url('https://files.catbox.moe/gimgy8.png');
        background-color: rgba(1,1,1,0.5)
    }
    .coneimg {
        width: 30px;
        height: 30px;
    }
    .bt {
    	background-color:#FF5F15;
        border-color:#FF5F15
    }
    .actiondiv {
    	display:flex;
    }
</style>
<html>
    <head>
        <title>cones | CSL</title>
    </head>
<body>

<h1 style="margin-bottom:3px; color:#FF5F15">CONES SAVE LIVES</h1>
<h2 style="padding-left:10px; margin-top:0px; background-color:#FF5F15; color:white">so lets save theirs.</h2>

<p style="color:grey">cones are currently facing the risk of erasion worldwide due to the harsh acts of the ATA (Anti-Cone Assosiation). We can only save them with your help. every press matters.</p>

<div class="actiondiv">
    <button class="bt" onclick="saveacone()">save a cone</button>
    <p class="cs" style="color:grey; margin-top:4px; margin-bottom:4px; padding-left:6px">cones saved: 0</p>
</div>

<p style='color:lightgrey'>below is a visual reperesentation of all the cones saved thanks to the communities help.</p>

<div class='allthecones' style="background-color:white; display:flex; flex-wrap: wrap;">
</div>

</body>
</html>

<script>
const cs = document.getElementsByClassName('cs')[0]
const bt = document.getElementsByClassName('bt')[0]
const div = document.getElementsByClassName('actiondiv')[0]
const allcones = document.getElementsByClassName('allthecones')[0]

function atc(num) {
    allcones.textContent = ""
    const coneimglist = [
        'https://www.rpmhardware.com/image/cache//x/2/x23e8qcvj_2604000-600x600.jpg',
        'https://www.rpmhardware.com/image/cache//x/2/x23e8qcvj_1446287-800x800.jpg',
        'https://www.rpmhardware.com/image/cache//x/2/x23e8qcvj_2605508-800x800.jpg',
        'https://www.rpmhardware.com/image/cache//x/2/x23e8qcvj_2607209-800x800.jpg',
        'https://www.rpmhardware.com/image/cache//x/2/x23e8qcvj_3522450-800x800.jpg'
    ]
    if (num) {
        for (let i = 0; i < num; i++) {
            const img = document.createElement('img')
            
            img.src = coneimglist[i - (Math.floor((i/5))*5)]
            img.alt = 'a cone that has been saved.'
            img.className = 'coneimg'
            //img.width = '30px'
            //img.height = '30px'
            allcones.appendChild(img)
        }
    }
}

async function getsavedcones() {
    try {
        let c = await fetch("https://ikelene.dev/storage/get.php", {
            headers: {
                "accept": "application/json",
                "content-type": "application/json"
            },
            body: "{\"apiKey\":\"d7d1607ac9036f65b3a25202f0d24aa9bfe01a25\",\"key\":\"cone\"}",
            method: "POST",
            credentials: "omit"
        });
        c = await c.json()
        const current = Number(c.data.value)
        atc(Number(current))
        return current
    } catch (err) {
        return null
    }
}

async function saveacone() {
    try {
        bt.disabled = true
        let current = await getsavedcones()

        if (!current) { return }
        let s = fetch("https://ikelene.dev/storage/store.php", {
            headers: {
                "accept": "application/json",
                "content-type": "application/json"
            },
            body: `{\"apiKey\":\"d7d1607ac9036f65b3a25202f0d24aa9bfe01a25\",\"key\":\"cone\",\"value\":\"${current + 1}\",\"mimeType\":\"application/json\"}`,
            method: "POST",
            credentials: "omit"
        });
        s = (await s).json()

        const now = await getsavedcones()

        cs.textContent = 'cones saved: ' + now

        setTimeout(() => {
            bt.disabled = false
        }, 10000);
    } catch (err) {
        if (err) {
            console.log(err)
            cs.textContent = 'there was a connection error. please try again later'
        }
    }
}

(async () => {
    div.style = "display:none"
    const start = await getsavedcones()

    if (start) {
        cs.textContent = 'cones saved: ' + start
        div.style = "display:flex"
    } else {
        cs.disabled = true
        cs.textContent = 'there was a problem with your connection. please reload'
        bt.remove()
        div.style = "display:flex"
    }

    setInterval(async () => {
        const updated = await getsavedcones()
        if (updated) {
            cs.textContent = 'cones saved: ' + updated

        }
    }, 30000);
})()

</script>

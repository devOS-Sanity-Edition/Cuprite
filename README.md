# Cuprite

<p align="center">
  <img src="docs/assets/Arc_NAmemCD7uP.png" width="512"></img>
  <img src="docs/assets/Arc_H1SxFkFD7F.png" width="512"></img>
</p>

Cuprite is a rounded corners theme designed for Writerside documentation. The point is to make it look simplistic and as clean as with some other visual hints and animation to adminitions and cards.

If you want to see how Cuprite looks in a live environment, you can view the [Yiski documentation](https://yiski.devos.one).

> [!NOTE]
> We do not support Algolia search as we don't have a key, so the theme is likely to look off with Search functions. Sorry about that. This may change in the future though.

## Usage

> [!IMPORTANT]
> This is meant to be used with Writerside 2024.1 EAP as of the time of writing, older versions of Writerside will not be supported!

Open your Writerside project and go to your `Writerside/cfg/buildprofiles.xml`, and allow Custom CSS by adding to your Build Profile's Variables, and adding a Link Color and Primary Color to your Variables too, like so

```xml
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE buildprofiles SYSTEM "https://resources.jetbrains.com/writerside/1.0/build-profiles.dtd">
<buildprofiles xsi:noNamespaceSchemaLocation="https://resources.jetbrains.com/writerside/1.0/build-profiles.xsd"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">

    <variables></variables>
    <build-profile instance="docs">
        <variables>
            <primary-color>#F75D62</primary-color>
            <link-color>#F75D62</link-color>
            <custom-css>custom.css</custom-css>
        </variables>
        </footer>
    </build-profile>

</buildprofiles>
```

Now under `Writerside/cfg`, make a new folder called `static`, and then a file named `custom.css`. Writerside will now pull that Custom CSS file.

On the top, add this if you want *all* of the CSS tweaks Cuprite makes

```css
@import "https://raw.githubusercontent.com/devOS-Sanity-Edition/Cuprite/main/Cuprite.css";
```

After that, add the following to your Custom CSS file

```css
:root {
    /* REPLACE 247, 92, 98 WITH YOUR BRANDING'S COLOR IN RGB */
    --actual-primary-color: 247, 93, 98;
}
```

Individual tweaks will be available at a later date.

## Screenshots

![image](docs/assets/Arc_VMyPaUbmMO.png)
![image](docs/assets/Arc_3d4K6OCOx4.png)
![image](docs/assets/Arc_yIJNO8yRUV.png)
![image](docs/assets/Arc_a7pomVA0BI.png)
![image](docs/assets/Arc_HjGehq5Lfe.png)
![image](docs/assets/Arc_jHX4o5iRke.png)
![image](docs/assets/Arc_kdpYC7KLun.png)
![image](docs/assets/Arc_utlX3BAPVd.png)
![image](docs/assets/Arc_wKKhL1OPRB.png)
![image](docs/assets/Arc_mRvuWDuTPt.png)
![image](docs/assets/Arc_yNR8n8bmBS.png)

## Videos

![video](docs/assets/Arc_0LWw56574s.mp4)
![video](docs/assets/Arc_dOcSgoPasM.mp4)
![video](docs/assets/Arc_UXSKlaAANe.mp4)

## License
This project is licensed under the [MIT License](LICENSE).
# TravelBus Anaylzer Desktop Application (Linux Release)

Public release of TravelBus Analyzer desktop application for Acute's TravelBus products.

**_NOTE:_** The application on Linux platform are still marked as beta versions. Please create an issue if you encounter any errors when running the program.

## Supported Models

| Types                        | Product                                       |
| ---------------------------- | --------------------------------------------- |
| Logic Analyzer               | Acute TravelBus 3000 series<br>Acute TravelBus 2000 series<br>Acute TravelBus 1000 series                 |

## Supported Operating System

Ubuntu 18.04+ (Bionic Beaver)

## Download TravelBus Analyzer

Download the latest version of the application from the [**Releases**](https://github.com/acute-technology-inc/tba-release/releases/latest) page.

TravelBus Analyzer application is provided in an **AppImage** format, and all previous versions can also be found in the release page.

## Update TravelBus Analyzer

One can update it manually by downloading the latest version of the application.

Or, you can use [**AppImageUpdate**](https://github.com/AppImageCommunity/AppImageUpdate) GUI tool to update the application.
See also [Making AppImages updateable](https://docs.appimage.org/packaging-guide/optional/updates.html#via-appimageupdate-built-into-the-appimage).

## Instructions

AppImages requires making the file into executable before using it.

Check the box that says **Allow executing file as program** as shown in the image.

![Demo Image](https://github.com/acute-technology-inc/tba-release/blob/main/res/image.png?raw=true)

Or, you can type

```
    chmod a+x TravelBus_Analyzer-x86_64.AppImage
```

Simply double-click the file to launch the application after the file is changed into an executable file.

Next, the application requires udev rules to allow non-root access to Acute’s
devices. Thus, you may need to install the udev rule file that you can obtain from
`LinuxSoftwareResources.tar.gz`.

1.	Download the udev file.
2.	Type the following command in the terminal.

    ```
    sudo cp 99-AcuteUSB.rules /etc/udev/rules.d
    ```

3.	Restart PC.
4.	Launch the application.

## Troubleshooting

See [Troubleshooting guide](https://github.com/acute-technology-inc/tba-release/blob/main/TROUBLESHOOTING.md) if you encounter any issues regarding the application.

# BasicThemer3
Mostly just basicthemer2 but applies instantly to windows without the need for them to be in focus first.
This is achieved by calling DwmSetWindowAttribute every millisecond for every open window, as opposed to BasicThemer2 which only calls it once when the window is in focus. As a result, this is slightly heavier but of course provides a much more seamless basic theme experience. However it's also lighter in some ways.
Full feature list:

• Basic theme is applied to all open windows immediately

• Very lightweight (11 kb)

• No taskbar icon

• Authentic looking description (of course you can change it with Resource Hacker)

![Screenshot showing description and size](https://user-images.githubusercontent.com/84914212/200675676-7d2274cd-151c-46c4-b90c-68644cc7f411.png)

**Edge/Chrome buggy titlebar?**

If you don't want to use Windows 10 titlebar in Edge and Chrome with this enabled, you can also use <a href="https://chrome.google.com/webstore/detail/windows-vista-basic-theme/bkohfcingfpclphbaglfbbjbfajcepad">this theme</a> to apply this basic colors and activate Edge/Chrome legacy theme. Note you still need to have the **-disable-windows10-custom-titlebar** in the shortcut. If you don't want to use this theme you can use the flag **-disable-gpu-compositing** but of course this is not recommended because then GPU will not be used at all.


**Window shows Windows theme when not responding**

To prevent DWM from showing the Windows theme when a window becomes not responding, simply rename DWMGhost.dll in System32 to anything else (you will have to take ownership of the file). This also disables the white effect that is applied on top of a window when it's not responding.


You can place it in System32 folder for maximum looking authenticity

Most credit for this program goes to pb-cairo. Idk why he doesn't maintain it because it is very nice, but he gave me permission to share and edit it.

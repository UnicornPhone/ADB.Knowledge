guide:
- https://stackoverflow.com/questions/25271878/android-adbd-cannot-run-as-root-in-production-builds

# Discuss:
https://xdaforums.com/t/2014-11-10-root-adbd-insecure-v2-00.1687590/

## Comment:
[Jul 11, 2024](https://xdaforums.com/t/2014-11-10-root-adbd-insecure-v2-00.1687590/page-15#post-89605771)
>Here is what I have discovered:
>
>Any manipulation of the ro.debuggable= set to "1" on A14 will allow adb as root but will crash the Developer Console menu in settings. To avoid that set SELinux to permissive. The developer menu will show but while it is open the CPU usage will increase dramatically. Maybe someone can figure why this occurs.
>
>I use a "ADB Root Enabler" magisk module in KernelSU in conjunction with SelinuxModeChange toggle app to do what I need in ADB as root, then I disable both when I'm done.
>
>Lastly will there be support for A14 in adbd insecure?

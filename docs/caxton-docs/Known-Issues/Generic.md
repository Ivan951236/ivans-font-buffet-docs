# Generic Modpack Issues + Generic Modpack FAQ

Q1: My Modpack has just crashed unexpectably after installing a mod, is it the mod or the mod loader?!?!?!

A1: If the Modpack crashes unexpectably after installing another mod to the Modpack, identify which mod crashed it first,
in this example (aka in this log), I am looking for TitleChanger Next, since this is the only mod I Installed after playing around with some mods, as I know it caused the crash
It should look like this in line 784:

```
767|[13:11:38] [Render thread/ERROR]: Reported exception thrown!
768|net.minecraft.class_148: Rendering overlay
769|at knot/net.minecraft.class_757.method_3192(class_757.java:545) ~[client-intermediary.jar:?]
770|at knot/net.minecraft.class_310.method_1523(class_310.java:1361) ~[client-intermediary.jar:?]
771|at knot/net.minecraft.class_310.method_1514(class_310.java:947) [client-intermediary.jar:?]
772|at knot/net.minecraft.client.main.Main.main(Main.java:265) [client-intermediary.jar:?]
773|at net.fabricmc.loader.impl.game.minecraft.MinecraftGameProvider.launch(MinecraftGameProvider.java:506) [fabric-loader-0.17.2.jar:?]
774|at net.fabricmc.loader.impl.launch.knot.Knot.launch(Knot.java:72) [fabric-loader-0.17.2.jar:?]
775|at net.fabricmc.loader.impl.launch.knot.KnotClient.main(KnotClient.java:23) [fabric-loader-0.17.2.jar:?]
776|at org.prismlauncher.launcher.impl.StandardLauncher.launch(StandardLauncher.java:105) [NewLaunch.jar:?]
777|at org.prismlauncher.EntryPoint.listen(EntryPoint.java:129) [NewLaunch.jar:?]
778|at org.prismlauncher.EntryPoint.main(EntryPoint.java:70) [NewLaunch.jar:?]
779|Caused by: java.lang.IllegalStateException: Can only blur once per frame
780|at knot/net.minecraft.class_11246.method_71299(class_11246.java:46) ~[client-intermediary.jar:?]
781|at knot/net.minecraft.class_332.method_71278(class_332.java:111) ~[client-intermediary.jar:?]
782|at knot/net.minecraft.class_437.method_57734(class_437.java:391) ~[client-intermediary.jar:?]
783|at knot/net.minecraft.class_437.method_25420(class_437.java:384) ~[client-intermediary.jar:?]
784|at knot/me.mmmjjkx.titlechanger.fabric.screens.LaunchScreen.method_25394(LaunchScreen.java:108) ~[titlechanger-fabric-2.0.6.jar:?]
785|at knot/net.minecraft.class_437.method_47413(class_437.java:113) ~[client-intermediary.jar:?]
786|at knot/net.minecraft.class_425.method_25394(class_425.java:82) ~[client-intermediary.jar:?]
787|at knot/net.minecraft.class_757.method_3192(class_757.java:538) ~[client-intermediary.jar:?]
```

In this case, it is the only mod I just installed, also the modpack does include "Crash Assistant" which allows you to upload and access your logs easily!

In the cases that it is the mod that came with the modpack, please report the issue to the issue tracker and it might be solved the first hour.

Q2: Where can I get my logs?

A2: Since this modpack does come with Crash Assistant, you can either upload it to a log-bin, like mclo.gs or gnomebot.dev, or instead you can access it locally and upload manually

Q3: May I please disable the bran-

A3: **NO**

Q4: I do know that after installing mods, modpack crashes, however I do not know which mod, help me!

A4: Please seperate the installed mods and the mods that came with the modpack and find out and uninstall those mods you installed, there is a modlist you can use to seperate yourself in this documentation

You can also read the log manually to see which mod by looking for the mod's filename as the culprit, try it with all mods you Installed, and if it does look like a error to you, please uninstall the offending mods

after that, you can try to upload the modpack's log to the mod's issue tracker hoping that the mod makes it compatible with the modpack, however if the mod was meant to be incompatible with one of the mods in this modpack, then you are out of luck.

Q5: Can I try to make a request to add another mod to the modpack?

A5: It depends, if the mod is lightweight enough and is also useful enough, then we can take it, as this modpack is meant to be lightweight, however if it too heavy in either size or performance or both, then we cannot take it.

It has to be lightweight enough to run nicely on Nvidia GeForce GTX 1660 Super and Intel Core i7 6700 combo, with 16GB of RAM and a terabyte of storage with generally no lower than 45 FPS would be great

The actual bare mininum is for my gaming rig not to crash even right after loading a world which is a Nvidia GeForce GTX 760 with Intel Core i5 2400, 8GB of RAM and a terabyte of total storage

Q6: Why is gaming rig so old and slow?

A6: Being poor is a factor too. `*cries in poor*`

Q7: May I please install shaders in this modpack?

A7: You may not, and the punishment is the same as disabling the modpack's branding which is told in the branding resource pack's descripition

The content of its manifest reads:

```
{
  "pack": {
    "pack_format": 64,
    "description": "§lDO NOT DISABLE, IF WE FIND OUT, THEN WE MAY BE ABLE TO REFUSE TO GIVE YOU BETA VERSIONS OF THIS MODPACK, PLUS YOU WILL NOT BE ABLE TO ACCESS THE DOCUMENTATION REPOSITORY SOURCE CODE",
    "supported_formats": {
      "min_inclusive": 30,
      "max_inclusive": 999
    }
  }
}
```

Q8: Can I actually use it with my own local server?

A8: any server works, any server hoster softwares works as well, like Purpur, Paper and Bukkit, and also any Online Server hosting site such as Modrinth Servers (the .modrinth.gg servers), Hypixel (with Microsoft Account), Medal and more also supported! (offline (aka cracked) servers also works)

However, your server must include the mod's own version for those server hosters to use properly, just like how Simple Voice Chat has a plugin for Paper server hosting software that has be to installed on the server for everyone to hear you.

Q9: Are all datapacks supported?

A9: Of course they are supported, this is because datapacks is just like minecraft's own official mod loader for singleplayer worlds only, they cannot access the mod-loader directly, so they act like normal,

this is unless the datapack requires andrew's datapack utils, in which case, they can access directly just to use its features.

Q10: Can you actually access the web from minecraft?

A10: It does require a mod that isn't in the modpack, so you must install the mod for it, to make it work, the mod name's is I don't really remember, but the mod is indeed there and still getting updates.


Modpack Exclusive Issues and FAQ isn't there yet, if a new Modpack specfic issues happends, please let me know and I will update the documentation for it.
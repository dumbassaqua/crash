---- Minecraft Crash Report ----
// This doesn't make any sense!

Time: 2022-08-22 19:55:44 EDT
Description: Exception in server tick loop

net.minecraftforge.fml.common.LoaderExceptionModCrash: Caught exception from EnderStorage (enderstorage)
Caused by: java.lang.RuntimeException: EnderStorage was unable to read it's data, please delete the 'EnderStorage' folder Here: C:\Users\24win\curseforge\minecraft\Instances\MC  Eternal\saves\rawr\EnderStorage and start the server again.
    at codechicken.enderstorage.manager.EnderStorageManager.load(EnderStorageManager.java:113)
    at codechicken.enderstorage.manager.EnderStorageManager.<init>(EnderStorageManager.java:78)
    at codechicken.enderstorage.manager.EnderStorageManager.reloadManager(EnderStorageManager.java:145)
    at codechicken.enderstorage.EnderStorage.preServerStart(EnderStorage.java:62)
    at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
    at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:497)
    at net.minecraftforge.fml.common.FMLModContainer.handleModStateEvent(FMLModContainer.java:637)
    at sun.reflect.GeneratedMethodAccessor5.invoke(Unknown Source)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:497)
    at com.google.common.eventbus.Subscriber.invokeSubscriberMethod(Subscriber.java:91)
    at com.google.common.eventbus.Subscriber$SynchronizedSubscriber.invokeSubscriberMethod(Subscriber.java:150)
    at com.google.common.eventbus.Subscriber$1.run(Subscriber.java:76)
    at com.google.common.util.concurrent.MoreExecutors$DirectExecutor.execute(MoreExecutors.java:399)
    at com.google.common.eventbus.Subscriber.dispatchEvent(Subscriber.java:71)
    at com.google.common.eventbus.Dispatcher$PerThreadQueuedDispatcher.dispatch(Dispatcher.java:116)
    at com.google.common.eventbus.EventBus.post(EventBus.java:217)
    at net.minecraftforge.fml.common.LoadController.sendEventToModContainer(LoadController.java:219)
    at net.minecraftforge.fml.common.LoadController.propogateStateMessage(LoadController.java:197)
    at sun.reflect.GeneratedMethodAccessor40.invoke(Unknown Source)
    at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
    at java.lang.reflect.Method.invoke(Method.java:497)
    at com.google.common.eventbus.Subscriber.invokeSubscriberMethod(Subscriber.java:91)
    at com.google.common.eventbus.Subscriber$SynchronizedSubscriber.invokeSubscriberMethod(Subscriber.java:150)
    at com.google.common.eventbus.Subscriber$1.run(Subscriber.java:76)
    at com.google.common.util.concurrent.MoreExecutors$DirectExecutor.execute(MoreExecutors.java:399)
    at com.google.common.eventbus.Subscriber.dispatchEvent(Subscriber.java:71)
    at com.google.common.eventbus.Dispatcher$PerThreadQueuedDispatcher.dispatch(Dispatcher.java:116)
    at com.google.common.eventbus.EventBus.post(EventBus.java:217)
    at net.minecraftforge.fml.common.LoadController.distributeStateMessage(LoadController.java:136)
    at net.minecraftforge.fml.common.Loader.serverStarted(Loader.java:804)
    at net.minecraftforge.fml.common.FMLCommonHandler.handleServerStarted(FMLCommonHandler.java:302)
    at net.minecraft.server.MinecraftServer.run(MinecraftServer.java:488)
    at java.lang.Thread.run(Thread.java:745)
Caused by: java.util.zip.ZipException: Not in GZIP format
    at java.util.zip.GZIPInputStream.readHeader(GZIPInputStream.java:165)
    at java.util.zip.GZIPInputStream.<init>(GZIPInputStream.java:79)
    at java.util.zip.GZIPInputStream.<init>(GZIPInputStream.java:91)
    at net.minecraft.nbt.CompressedStreamTools.readCompressed(CompressedStreamTools.java:26)
    at codechicken.enderstorage.manager.EnderStorageManager.load(EnderStorageManager.java:104)
    ... 35 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
  Minecraft Version: 1.12.2
  Operating System: Windows 10 (amd64) version 10.0
  Java Version: 1.8.0_51, Oracle Corporation
  Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
  Memory: 1332751352 bytes (1271 MB) / 9123659776 bytes (8701 MB) up to 11453595648 bytes (10923 MB)
  JVM Flags: 3 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx12288m -Xms256m
  IntCache: cache: 16, tcache: 0, allocated: 5, tallocated: 104
  FML: MCP 9.42 Powered by Forge 14.23.5.2854 378 mods loaded, 376 mods active
       States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
       
       | State   | ID                                | Version                  | Source                                            | Signature                                |
       |:------- |:--------------------------------- |:------------------------ |:------------------------------------------------- |:---------------------------------------- |
       | LCHIJA  | minecraft                         | 1.12.2                   | minecraft.jar                                     | None                                     |
       | LCHIJA  | mcp                               | 9.42                     | minecraft.jar                                     | None                                     |
       | LCHIJA  | FML                               | 8.0.99.99                | forge-1.12.2-14.23.5.2854.jar                     | e3c3d50c7c986df74c645c0ac54639741c90a557 |
       | LCHIJA  | forge                             | 14.23.5.2854             | forge-1.12.2-14.23.5.2854.jar                     | e3c3d50c7c986df74c645c0ac54639741c90a557 |
       | LCHIJA  | advancedrocketrycore              | 1                        | minecraft.jar                                     | None                                     |
       | LCHIJA  | ColorUtility                      | 1.0.4                    | minecraft.jar                                     | None                                     |
       | LCHIJA  | creativecoredummy                 | 1.0.0                    | minecraft.jar                                     | None                                     |
       | LCHIJA  | ivtoolkit                         | 1.3.3-1.12               | minecraft.jar                                     | None                                     |
       | LCHIJA  | littletilescore                   | 1.0.0                    | minecraft.jar                                     | None                                     |
       | LCHIJA  | openmodscore                      | 0.12.2                   | minecraft.jar                                     | None                                     |
       | LCHIJA  | foamfixcore                       | 7.7.4                    | minecraft.jar                                     | None                                     |
       | LCHIJA  | obfuscate                         | 0.4.2                    | minecraft.jar                                     | None                                     |
       | LCHIJA  | opencomputers|core                | 1.7.5.192                | minecraft.jar                                     | None                                     |
       | LCHIJA  | randompatches                     | 1.12.2-1.22.1.10         | randompatches-1.12.2-1.22.1.10.jar                | None                                     |
       | LCHIJA  | tweakersconstruct                 | 1.12.2-1.6.0             | tweakersconstruct-1.12.2-1.6.0.jar                | None                                     |
       | LCHIJA  | fastbench                         | 1.7.3                    | FastWorkbench-1.12.2-1.7.3.jar                    | None                                     |
       | LCHIJA  | actuallyadditions                 | 1.12.2-r152              | ActuallyAdditions-1.12.2-r152.jar                 | None                                     |
       | LCHIJA  | forgeendertech                    | 1.12.2-4.5.5.0           | ForgeEndertech-1.12.2-4.5.5.0-build.0561.jar      | None                                     |
       | LCHIJA  | adhooks                           | 1.12.2-3.3.0.0           | AdHooks-1.12.2-3.3.0.0-build.0528.jar             | None                                     |
       | LCHIJA  | adlods                            | 1.12.2-1.0.8.0           | AdLods-1.12.2-1.0.8.0-build.0504.jar              | None                                     |
       | LCHIJA  | redstoneflux                      | 2.1.1                    | RedstoneFlux-1.12-2.1.1.1-universal.jar           | None                                     |
       | LCHIJA  | cofhcore                          | 4.6.6                    | CoFHCore-1.12.2-4.6.6.1-universal.jar             | None                                     |
       | LCHIJA  | libvulpes                         | 0.4.2.-75                | LibVulpes-1.12.2-0.4.2-75-universal.jar           | None                                     |
       | LCHIJA  | advancedrocketry                  | 1.7.0.-232               | AdvancedRocketry-1.12.2-1.7.0-232-universal.jar   | None                                     |
       | LCHIJA  | ctm                               | MC1.12.2-1.0.2.31        | CTM-MC1.12.2-1.0.2.31.jar                         | None                                     |
       | LCHIJA  | appliedenergistics2               | rv6-stable-7             | appliedenergistics2-rv6-stable-7.jar              | dfa4d3ac143316c6f32aa1a1beda1e34d42132e5 |
       | LCHIJA  | bdlib                             | 1.14.3.12                | bdlib-1.14.3.12-mc1.12.2.jar                      | None                                     |
       | LCHIJA  | ae2stuff                          | 0.7.0.4                  | ae2stuff-0.7.0.4-mc1.12.2.jar                     | None                                     |
       | LCHIJA  | baubles                           | 1.5.2                    | Baubles-1.12-1.5.2.jar                            | None                                     |
       | LCHIJA  | roots                             | 1.12.2-3.0.33            | Roots-1.12.2-3.0.33.jar                           | None                                     |
       | LCHIJA  | mysticalworld                     | 1.12.2-1.9.8             | mysticalworld-1.12.2-1.9.8.jar                    | None                                     |
       | LCHIJA  | endercore                         | 1.12.2-0.5.76            | EnderCore-1.12.2-0.5.76.jar                       | None                                     |
       | LCHIJA  | crafttweaker                      | 4.1.20                   | CraftTweaker2-1.12-4.1.20.618.jar                 | None                                     |
       | LCHIJA  | mtlib                             | 3.0.6                    | MTLib-3.0.6.jar                                   | None                                     |
       | LCHIJA  | modtweaker                        | 4.0.18                   | modtweaker-4.0.18.jar                             | None                                     |
       | LCHIJA  | jei                               | 4.16.1.301               | jei_1.12.2-4.16.1.301.jar                         | None                                     |
       | LCHIJA  | thaumcraft                        | 6.1.BETA26               | Thaumcraft-1.12.2-6.1.BETA26.jar                  | None                                     |
       | LCHIJA  | codechickenlib                    | 3.2.3.358                | CodeChickenLib-1.12.2-3.2.3.358-universal.jar     | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LCHIJA  | cofhworld                         | 1.4.0                    | CoFHWorld-1.12.2-1.4.0.1-universal.jar            | None                                     |
       | LCHIJA  | thermalfoundation                 | 2.6.7                    | ThermalFoundation-1.12.2-2.6.7.1-universal.jar    | None                                     |
       | LCHIJA  | thermalexpansion                  | 5.5.7                    | ThermalExpansion-1.12.2-5.5.7.1-universal.jar     | None                                     |
       | LCHIJA  | enderio                           | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | mantle                            | 1.12-1.3.3.55            | Mantle-1.12-1.3.3.55.jar                          | None                                     |
       | LCHIJA  | chisel                            | MC1.12.2-1.0.2.45        | Chisel-MC1.12.2-1.0.2.45.jar                      | None                                     |
       | LCHIJA  | enderiointegrationtic             | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | tombstone                         | 4.1.2                    | tombstone-4.1.2-1.12.2.jar                        | None                                     |
       | LCHIJA  | quark                             | r1.6-179                 | Quark-r1.6-179.jar                                | None                                     |
       | LCHIJA  | twilightforest                    | 3.11.1021                | twilightforest-1.12.2-3.11.1021-universal.jar     | None                                     |
       | LCHIJA  | tconstruct                        | 1.12.2-2.13.0.183        | TConstruct-1.12.2-2.13.0.183.jar                  | None                                     |
       | LCHIJA  | p455w0rdslib                      | 2.3.161                  | p455w0rdslib-1.12.2-2.3.161.jar                   | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LCHIJA  | ae2wtlib                          | 1.0.34                   | AE2WTLib-1.12.2-1.0.34.jar                        | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LCHIJA  | infinitylib                       | 1.12.2-1.12.0            | infinitylib-1.12.0.jar                            | None                                     |
       | LCHIJA  | agricraft                         | 2.12.0-1.12.0-a6         | AgriCraft-2.12.0-1.12.0-a6.jar                    | None                                     |
       | LCHIJA  | aiimprovements                    | 0.0.1.3                  | AIImprovements-1.12-0.0.1b3.jar                   | None                                     |
       | LCHIJA  | akashictome                       | 1.2-12                   | AkashicTome-1.2-12.jar                            | None                                     |
       | LCHIJA  | creativecore                      | 1.10.0                   | CreativeCore_v1.10.47_mc1.12.2.jar                | None                                     |
       | LCHIJA  | ambientsounds                     | 3.0                      | AmbientSounds_v3.1.5_mc1.12.2.jar                 | None                                     |
       | LCHIJA  | ebwizardry                        | 4.3.4                    | ElectroblobsWizardry-4.3.4-MC1.12.2.jar           | None                                     |
       | LCHIJA  | ancientspellcraft                 | 1.1.3                    | ancientspellcraft-1.1.3.jar                       | None                                     |
       | LCHIJA  | ancientwarfare                    | 1.12.2-2.7.0.1032        | ancientwarfare-1.12.2-2.7.0.1032.jar              | None                                     |
       | LCHIJA  | buildcraftlib                     | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | buildcraftcore                    | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | ancientwarfareautomation          | 1.12.2-2.7.0.1032        | ancientwarfare-1.12.2-2.7.0.1032.jar              | None                                     |
       | LCHIJA  | ancientwarfarenpc                 | 1.12.2-2.7.0.1032        | ancientwarfare-1.12.2-2.7.0.1032.jar              | None                                     |
       | LCHIJA  | ancientwarfarestructure           | 1.12.2-2.7.0.1032        | ancientwarfare-1.12.2-2.7.0.1032.jar              | None                                     |
       | LCHIJA  | ancientwarfarevehicle             | 1.12.2-2.7.0.1032        | ancientwarfare-1.12.2-2.7.0.1032.jar              | None                                     |
       | LCHIJA  | applecore                         | 3.4.0                    | AppleCore-mc1.12.2-3.4.0.jar                      | None                                     |
       | LCHIJA  | appleskin                         | 1.0.14                   | AppleSkin-mc1.12-1.0.14.jar                       | None                                     |
       | LCHIJA  | architecturecraft                 | @VERSION@                | architecturecraft-1.12-3.98.jar                   | None                                     |
       | LCHIJA  | conarm                            | 1.2.5.10                 | conarm-1.12.2-1.2.5.10.jar                        | b33d2c8df492beff56d1bbbc92da49b8ab7345a1 |
       | LCHIJA  | armoryexpansion                   | 1.4.2                    | armoryexpansion-1.4.2.jar                         | None                                     |
       | LCHIJA  | armoryexpansion-custommaterials   | 1.4.2                    | armoryexpansion-1.4.2.jar                         | None                                     |
       | LCHIJA  | hammercore                        | 2.0.6.26                 | HammerLib-1.12.2-2.0.6.26.jar                     | 9f5e2a811a8332a842b34f6967b7db0ac4f24856 |
       | LCHIJA  | thaumadditions                    | 12.6.6                   | ThaumicAdditions-1.12.2-12.6.6.jar                | 9f5e2a811a8332a842b34f6967b7db0ac4f24856 |
       | LCHIJA  | llibrary                          | 1.7.20                   | llibrary-1.7.20-1.12.2.jar                        | b9f30a813bee3b9dd5652c460310cfcd54f6b7ec |
       | LCHIJA  | iceandfire                        | 1.9.1                    | iceandfire-1.9.1-1.12.2.jar                       | None                                     |
       | LCHIJA  | armoryexpansion-iceandfire        | 1.4.2                    | armoryexpansion-1.4.2.jar                         | None                                     |
       | LCHIJA  | armoryexpansion-matteroverdrive   | 1.4.2                    | armoryexpansion-1.4.2.jar                         | None                                     |
       | LCHIJA  | aroma1997core                     | 2.0.0.2.b167             | Aroma1997Core-1.12.2-2.0.0.2.b167.jar             | dfbfe4c473253d8c5652417689848f650b2cbe32 |
       | LCHIJA  | aromabackup                       | 3.0.0.0.b135             | AromaBackup-1.12.2-3.0.0.0.b135.jar               | dfbfe4c473253d8c5652417689848f650b2cbe32 |
       | LCHIJA  | aromabackuprecovery               | 3.0.0.0.b135             | AromaBackup-1.12.2-3.0.0.0.b135.jar               | dfbfe4c473253d8c5652417689848f650b2cbe32 |
       | LCHIJA  | artifacts                         | 1.12.2-1.2.3             | Artifacts-1.12.2-1.2.3.jar                        | None                                     |
       | LCHIJA  | astralsorcery                     | 1.10.27                  | astralsorcery-1.12.2-1.10.27.jar                  | a0f0b759d895c15ceb3e3bcb5f3c2db7c582edf0 |
       | LCHIJA  | attributefix                      | 1.0.4                    | AttributeFix-1.12.2-1.0.4.jar                     | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LCHIJA  | atum                              | 2.0.20                   | Atum-1.12.2-2.0.20.jar                            | None                                     |
       | LCHIJA  | mdecore                           | 1.12-1.1                 | mdecore-1.12-1.1.jar                              | None                                     |
       | LCHIJA  | autooredictconv                   | 1.12-1.0.1               | autooredictconv-1.12-1.0.1.jar                    | None                                     |
       | LCHIJA  | autoreglib                        | 1.3-32                   | AutoRegLib-1.3-32.jar                             | None                                     |
       | LCHIJA  | badwithernocookiereloaded         | 1.12.2-3.4.18            | badwithernocookiereloaded-1.12.2-3.4.18.jar       | None                                     |
       | LCHIJA  | battletowers                      | 1.6.5                    | BattleTowers-1.12.2.jar                           | None                                     |
       | LCHIJA  | betterbuilderswands               | 0.13.2                   | BetterBuildersWands-1.12.2-0.13.2.271+5997513.jar | None                                     |
       | LCHIJA  | bettercaves                       | 1.12.2                   | bettercaves-1.12.2-2.0.4.jar                      | None                                     |
       | LCHIJA  | botania                           | r1.10-363                | Botania r1.10-363.jar                             | None                                     |
       | LCHIJA  | mowziesmobs                       | 1.5.8                    | mowziesmobs-1.5.8.jar                             | None                                     |
       | LCHIJA  | patchouli                         | 1.0-23.6                 | Patchouli-1.0-23.6.jar                            | None                                     |
       | LCHIJA  | bewitchment                       | 0.22.63                  | bewitchment-1.12.2-0.0.22.64.jar                  | None                                     |
       | LCHIJA  | bibliocraft                       | 2.4.5                    | BiblioCraft[v2.4.5][MC1.12.2].jar                 | None                                     |
       | LCHIJA  | biomeinfo                         | v1.2.5                   | biomeinfo-1.12.2-v1.2.5.jar                       | None                                     |
       | LCHIJA  | biomesoplenty                     | 7.0.1.2441               | BiomesOPlenty-1.12.2-7.0.1.2441-universal.jar     | None                                     |
       | LCHIJA  | biomestaff                        | 1.0.0                    | BiomeStaff-1.12.2-1.0.0.jar                       | None                                     |
       | LCHIJA  | blockdrops                        | 1.4.0                    | blockdrops-1.12.2-1.4.0.jar                       | None                                     |
       | LCHIJA  | cyclicmagic                       | 1.20.8                   | Cyclic-1.12.2-1.20.8.jar                          | 0e5cb559be7d03f3fc18b8cba547d663e25f28af |
       | LCHIJA  | guideapi                          | 1.12-2.1.8-63            | Guide-API-1.12-2.1.8-63.jar                       | None                                     |
       | LCHIJA  | bloodmagic                        | 1.12.2-2.4.3-105         | BloodMagic-1.12.2-2.4.3-105.jar                   | None                                     |
       | LCHIJA  | bookshelf                         | 2.3.590                  | Bookshelf-1.12.2-2.3.590.jar                      | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LCHIJA  | bountifulbaubles                  | 0.0.1                    | Bountiful Baubles-1.12.2-0.1.6.jar                | None                                     |
       | LCHIJA  | forgelin                          | 1.8.4                    | Forgelin-1.8.4.jar                                | None                                     |
       | LCHIJA  | bountiful                         | 2.2.2                    | Bountiful-2.2.2.jar                               | None                                     |
       | LCHIJA  | brokenwings                       | 2.0.0                    | brokenwings-3.0.0.jar                             | None                                     |
       | LCHIJA  | buildcraftbuilders                | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | buildcrafttransport               | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | buildcraftsilicon                 | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | buildcraftenergy                  | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | reborncore                        | 3.19.5                   | RebornCore-FORK-1.12.2-3.19.5-universal.jar       | None                                     |
       | LCHIJA  | techreborn                        | 2.27.3.1084              | TechReborn-1.12.2-2.27.3.1084-universal.jar       | 8727a3141c8ec7f173b87aa78b9b9807867c4e6b |
       | LCHIJA  | forestry                          | 5.8.2.422                | forestry_1.12.2-5.8.2.422.jar                     | None                                     |
       | LCHIJA  | buildcraftcompat                  | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | buildcraftfactory                 | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | buildcraftrobotics                | 7.99.24.8                | buildcraft-all-7.99.24.8.jar                      | None                                     |
       | LCHIJA  | buildinggadgets                   | 2.8.4                    | BuildingGadgets-2.8.4.jar                         | None                                     |
       | LCHIJA  | capsule                           | 1.12.2-3.3.11            | Capsule-1.12.2-3.3.11.jar                         | None                                     |
       | LCHIJA  | careerbees                        | 1.0                      | careerbees-0.4.0.jar                              | None                                     |
       | LCHIJA  | chameleon                         | 1.12-4.1.3               | Chameleon-1.12-4.1.3.jar                          | None                                     |
       | LCHIJA  | champions                         | 1.12.2-1.0.11.10         | champions-1.12.2-1.0.11.10.jar                    | b33d2c8df492beff56d1bbbc92da49b8ab7345a1 |
       | LCHIJA  | chancecubes                       | 1.12.2-5.0.2.385         | ChanceCubes-1.12.2-5.0.2.385.jar                  | None                                     |
       | LCHIJA  | charm                             | 1.4                      | Charm-1.12.2-1.4.1.jar                            | None                                     |
       | LCHIJA  | cherishedworlds                   | 1.12.2-1.0.1             | cherishedworlds-1.12.2-1.0.1.jar                  | 2484ef4d131fdc0dca0647aa21b7b944ddb935a1 |
       | LCHIJA  | chiselsandbits                    | 14.33                    | chiselsandbits-14.33.jar                          | None                                     |
       | LCHIJA  | chunkpregenerator                 | 2.5.0                    | Chunk Pregenerator-V1.12-2.5.0.jar                | None                                     |
       | LCHIJA  | clumps                            | 3.1.2                    | Clumps-3.1.2.jar                                  | None                                     |
       | LCHIJA  | collective                        | 2.25                     | collective-1.12.2-2.25.jar                        | None                                     |
       | LCHIJA  | cyclopscore                       | 1.6.7                    | CyclopsCore-1.12.2-1.6.7.jar                      | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LCHIJA  | commoncapabilities                | 2.4.8                    | CommonCapabilities-1.12.2-2.4.8.jar               | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LCHIJA  | compactmachines3                  | 3.0.18                   | compactmachines3-1.12.2-3.0.18-b278.jar           | None                                     |
       | LCHIJA  | controlling                       | 3.0.10                   | Controlling-3.0.10.jar                            | None                                     |
       | LCHIJA  | cookingforblockheads              | 6.5.0                    | CookingForBlockheads_1.12.2-6.5.0.jar             | None                                     |
       | LCHIJA  | cosmeticarmorreworked             | 1.12.2-v5a               | CosmeticArmorReworked-1.12.2-v5a.jar              | aaaf83332a11df02406e9f266b1b65c1306f0f76 |
       | LCHIJA  | craftingtweaks                    | 8.1.9                    | CraftingTweaks_1.12.2-8.1.9.jar                   | None                                     |
       | LCHIJA  | ctgui                             | 1.0.0                    | CraftTweaker2-1.12-4.1.20.618.jar                 | None                                     |
       | LCHIJA  | crafttweakerjei                   | 2.0.3                    | CraftTweaker2-1.12-4.1.20.618.jar                 | None                                     |
       | LCHIJA  | crimsonwarfare                    | 1.5                      | crimsonwarfare-1.5.jar                            | None                                     |
       | LCHIJA  | cucumber                          | 1.1.3                    | Cucumber-1.12.2-1.1.3.jar                         | None                                     |
       | LCHIJA  | culinaryconstruct                 | 1.3.4                    | culinaryconstruct-1.3.4.jar                       | 2484ef4d131fdc0dca0647aa21b7b944ddb935a1 |
       | LCHIJA  | customizeddungeonloot             | 1.0.3                    | Customized-Dungeon-Loot-1.12 -(v.1.0.3).jar       | None                                     |
       | LCHIJA  | custommainmenu                    | 2.0.9.1                  | CustomMainMenu-MC1.12.2-2.0.9.1.jar               | None                                     |
       | LCHIJA  | waila                             | 1.8.26                   | Hwyla-1.8.26-B41_1.12.2.jar                       | None                                     |
       | LCHIJA  | stg                               | 1.12.2-1.2.3             | stg-1.12.2-1.2.3.jar                              | None                                     |
       | LCHIJA  | mousetweaks                       | 2.10                     | MouseTweaks-2.10-mc1.12.2.jar                     | None                                     |
       | LCHIJA  | danknull                          | 1.7.101                  | DankNull-1.12.2-1.7.101.jar                       | 644f38521a349310a5dae0239577dc7beebefaec |
       | LCHIJA  | darknesslib                       | 1.1.0                    | DarknessLib-1.12.2-1.1.0.jar                      | 220f10d3a93b3ff5fbaa7434cc629d863d6751b9 |
       | LCHIJA  | dimdoors                          | 1.12.2-3.1.2+UNOFFICIAL  | DimensionalDoors-1.12.2-3.1.2-UNOFFICIAL.jar      | None                                     |
       | LCHIJA  | ding                              | 1.0.2                    | Ding-1.12.2-1.0.2.jar                             | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LCHIJA  | discordcraft                      | 1.0                      | DiscordCraft-2.0.jar                              | None                                     |
       | LCHIJA  | doggytalents                      | 1.15.1.6                 | DoggyTalents-1.12.2-1.15.1.6.jar                  | None                                     |
       | LCHIJA  | dungeonsmod                       | 1.12.2-1.0.6             | DungeonsMod-1.12.2-1.0.6.jar                      | None                                     |
       | LCHIJA  | dungeontactics                    | DT-0.16.9                | DungeonTactics-1.12.2-0.16.9.jar                  | None                                     |
       | LCHIJA  | eerieentities                     | 1.0.7                    | EerieEntities-1.12.2-1.0.7.jar                    | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LCHIJA  | elenaidodge2                      | 1.0.8b                   | ElenaiDodge2-1.12.2-1.0.8b.jar                    | None                                     |
       | LCHIJA  | enchdesc                          | 1.1.15                   | EnchantmentDescriptions-1.12.2-1.1.15.jar         | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LCHIJA  | enderiobase                       | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | enderioconduits                   | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | enderioconduitsappliedenergistics | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | opencomputers                     | 1.7.5.192                | OpenComputers-MC1.12.2-1.7.5.192.jar              | None                                     |
       | LCHIJA  | enderioconduitsopencomputers      | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | enderioconduitsrefinedstorage     | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | enderiointegrationforestry        | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | enderiointegrationticlate         | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | enderioinvpanel                   | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | ftblib                            | 5.4.7.2                  | FTBLib-5.4.7.2.jar                                | None                                     |
       | LCHIJA  | enderiomachines                   | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | enderiopowertools                 | 5.3.70                   | EnderIO-1.12.2-5.3.70.jar                         | None                                     |
       | LCHIJA  | mcmultipart                       | 2.5.3                    | MCMultiPart-2.5.3.jar                             | None                                     |
       | LCHIJA  | mekanism                          | 1.12.2-9.8.3.390         | Mekanism-1.12.2-9.8.3.390.jar                     | None                                     |
       | LCHIJA  | gasconduits                       | 5.3.70                   | EnderIO-conduits-mekanism-1.12.2-5.3.70.jar       | None                                     |
       | LCHIJAE | enderstorage                      | 2.4.6.137                | EnderStorage-1.12.2-2.4.6.137-universal.jar       | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LCHIJA  | energyconverters                  | 1.3.7.30                 | energyconverters_1.12.2-1.3.7.30.jar              | None                                     |
       | LCHIJA  | erebus                            | 1.0.32                   | Erebus-1.0.32.jar                                 | None                                     |
       | LCHIJA  | erebusfix                         | 1.12.2-0.0.0.1           | erebusfix-1.12.2-0.0.0.1.jar                      | None                                     |
       | LCHIJA  | extrabitmanipulation              | 1.12.2-3.4.1             | ExtraBitManipulation-1.12.2-3.4.1.jar             | None                                     |
       | LCHIJA  | extracells                        | 2.6.5                    | ExtraCells-1.12.2-2.6.5.jar                       | None                                     |
       | LCHIJA  | extrautils2                       | 1.0                      | extrautils2-1.12-1.9.9.jar                        | None                                     |
       | LCHIJA  | fairylights                       | 2.1.10                   | fairylights-2.2.0-1.12.2.jar                      | None                                     |
       | LCHIJA  | farmingforblockheads              | 3.1.28                   | FarmingForBlockheads_1.12.2-3.1.28.jar            | None                                     |
       | LCHIJA  | farseek                           | 2.5.1                    | Farseek-1.12-2.5.1.jar                            | None                                     |
       | LCHIJA  | mod_lavacow                       | 1.2.4                    | Fish's Undead Rising-1.2.4a.jar                   | None                                     |
       | LCHIJA  | sonarcore                         | 5.0.19                   | sonarcore-1.12.2-5.0.19-20.jar                    | None                                     |
       | LCHIJA  | fluxnetworks                      | 4.1.0                    | FluxNetworks-1.12.2-4.1.1.34.jar                  | None                                     |
       | LCHIJA  | foamfix                           | 0.10.14-1.12.2           | foamfix-0.10.14-1.12.2.jar                        | None                                     |
       | LCHIJA  | forgemultipartcbe                 | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar      | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LCHIJA  | microblockcbe                     | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar      | None                                     |
       | LCHIJA  | minecraftmultipartcbe             | 2.6.2.83                 | ForgeMultipart-1.12.2-2.6.2.83-universal.jar      | None                                     |
       | LCHIJA  | fossil                            | 8.0.5                    | fossilsarcheology-8.0.5.jar                       | None                                     |
       | LCHIJA  | from_the_depths                   | @VERSION@                | from_the_depths-1.2.1.0.jar                       | None                                     |
       | LCHIJA  | iceologer                         | 1.5                      | Frozen-Fiend-1.5.jar                              | None                                     |
       | LCHIJA  | ftbutilities                      | 5.4.1.131                | FTBUtilities-5.4.1.131.jar                        | None                                     |
       | LCHIJA  | itemfilters                       | 1.0.4.2                  | ItemFilters-1.0.4.2.jar                           | None                                     |
       | LCHIJA  | reskillable                       | 1.12.2-1.13.0            | Reskillable-1.12.2-1.13.0.jar                     | None                                     |
       | LCHIJA  | ftbquests                         | 1202.9.0.15              | FTBQuests-1202.9.0.15.jar                         | None                                     |
       | LCHIJA  | ftbmoney                          | 1.2.0.47                 | FTBMoney-1.2.0.47.jar                             | None                                     |
       | LCHIJA  | futuremc                          | 0.2.6                    | future-mc-1.12.2-0.2.6.1.jar                      | None                                     |
       | LCHIJA  | gendustry                         | 1.6.5.8                  | gendustry-1.6.5.8-mc1.12.2.jar                    | None                                     |
       | LCHIJA  | ghostsexplosives                  | 2.3.0 - MC 1.12.2        | Ghost's Explosives 2.3.0 - MC1.12.2.jar           | None                                     |
       | LCHIJA  | gottschcore                       | 1.14.0                   | GottschCore-mc1.12.2-f14.23.5.2854-v1.14.0.jar    | None                                     |
       | LCHIJA  | grue                              | 1.8.0                    | Grue-1.12.2-1.8.0.jar                             | 220f10d3a93b3ff5fbaa7434cc629d863d6751b9 |
       | LCHIJA  | guardillagers                     | 1.0.1                    | guardillagers-1.12.2-1.0.1.jar                    | None                                     |
       | LCHIJA  | gunpowderlib                      | 1.12.2-1.1               | GunpowderLib-1.12.2-1.1.jar                       | 4ffa87db52cf086d00ecc4853a929367b1c39b5c |
       | LCHIJA  | hardcoredarkness                  | 2.0                      | HardcoreDarkness-MC1.12.2-2.0.jar                 | d72e0dd57935b3e9476212aea0c0df352dd76291 |
       | LCHIJA  | ichunutil                         | 7.2.2                    | iChunUtil-1.12.2-7.2.2.jar                        | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LCHIJA  | hats                              | 7.1.1                    | Hats-1.12.2-7.1.1.jar                             | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LCHIJA  | hole_filler_mod                   | 1.0                      | hole_filler_mod-1.2.4.jar                         | None                                     |
       | LCHIJA  | hunterillager                     | 1.2                      | hunterillager-1.12.2-1.2.jar                      | None                                     |
       | LCHIJA  | icbmclassic                       | 1.12.2-4.0.1.75          | ICBM-classic-1.12.2-4.0.1b75.jar                  | None                                     |
       | LCHIJA  | illagers_plus                     | 1.1                      | IllagersPlus-1.12.2-1.1.3.jar                     | None                                     |
       | LCHIJA  | immersiveengineering              | 0.12-98                  | ImmersiveEngineering-0.12-98.jar                  | None                                     |
       | LCHIJA  | immersivecables                   | 1.3.2                    | ImmersiveCables-1.12.2-1.3.2.jar                  | None                                     |
       | LCHIJA  | immersiveintelligence             | 0.1.1                    | immersiveintelligence-1.12.2-0.1.1.jar            | None                                     |
       | LCHIJA  | immersivepetroleum                | 1.1.9                    | immersivepetroleum-1.12.2-1.1.9.jar               | None                                     |
       | LCHIJA  | immersiveposts                    | 0.2.1                    | ImmersivePosts-0.2.1.jar                          | 0ba8738eadcf158e7fe1452255a73a022fb15feb |
       | LCHIJA  | improvedbackpacks                 | 1.12.2-1.5.0.0           | ImprovedBackpacks-1.12.2-1.5.0.0.jar              | None                                     |
       | LCHIJA  | incontrol                         | 3.9.18                   | incontrol-1.12-3.9.18.jar                         | None                                     |
       | LCHIJA  | teslacorelib                      | 1.0.17                   | tesla-core-lib-1.12.2-1.0.17.jar                  | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LCHIJA  | industrialforegoing               | 1.12.2-1.12.2            | industrialforegoing-1.12.2-1.12.13-237.jar        | None                                     |
       | LCHIJA  | instantunify                      | 1.1.2                    | instantunify-1.12.2-1.1.2.jar                     | None                                     |
       | LCHIJA  | instrumentalmobs                  | 1.2                      | Instrumental-Mobs-1.2.1.jar                       | None                                     |
       | LCHIJA  | integrateddynamics                | 1.1.11                   | IntegratedDynamics-1.12.2-1.1.11.jar              | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LCHIJA  | integrateddynamicscompat          | 1.0.0                    | IntegratedDynamics-1.12.2-1.1.11.jar              | None                                     |
       | LCHIJA  | integratedtunnels                 | 1.6.14                   | IntegratedTunnels-1.12.2-1.6.14.jar               | bd0353b3e8a2810d60dd584e256e364bc3bedd44 |
       | LCHIJA  | integratedtunnelscompat           | 1.0.0                    | IntegratedTunnels-1.12.2-1.6.14.jar               | None                                     |
       | LCHIJA  | mysticalagriculture               | 1.7.5                    | MysticalAgriculture-1.12.2-1.7.5.jar              | None                                     |
       | LCHIJA  | mysticalagradditions              | 1.3.2                    | MysticalAgradditions-1.12.2-1.3.2.jar             | None                                     |
       | LCHIJA  | nuclearcraft                      | 2.18y                    | NuclearCraft-2.18y-1.12.2.jar                     | None                                     |
       | LCHIJA  | harvestcraft                      | 1.12.2zb                 | Pam's HarvestCraft 1.12.2zg.jar                   | None                                     |
       | LCHIJA  | randomthings                      | 4.2.7.4                  | RandomThings-MC1.12.2-4.2.7.4.jar                 | d72e0dd57935b3e9476212aea0c0df352dd76291 |
       | LCHIJA  | mcjtylib_ng                       | 3.5.4                    | mcjtylib-1.12-3.5.4.jar                           | None                                     |
       | LCHIJA  | rftools                           | 7.73                     | rftools-1.12-7.73.jar                             | None                                     |
       | LCHIJA  | integrationforegoing              | 1.12.2-1.11              | IntegrationForegoing-1.12.2-1.11.jar              | 4ffa87db52cf086d00ecc4853a929367b1c39b5c |
       | LCHIJA  | inventorypets                     | 2.0.12                   | inventorypets-1.12-2.0.12.jar                     | None                                     |
       | LCHIJA  | inventorytweaks                   | 1.63+release.109.220f184 | InventoryTweaks-1.63.jar                          | 55d2cd4f5f0961410bf7b91ef6c6bf00a766dcbe |
       | LCHIJA  | ironchest                         | 1.12.2-7.0.67.844        | ironchest-1.12.2-7.0.72.847.jar                   | None                                     |
       | LCHIJA  | itlt                              | 1.0.3                    | itlt-1.12.2-1.0.3.jar                             | None                                     |
       | LCHIJA  | jaopca                            | 1.12.2-2.2.8.103         | JAOPCA-1.12.2-2.2.8.103.jar                       | None                                     |
       | LCHIJA  | oredictinit                       | 1.12.2-2.2.1.71          | JAOPCA-1.12.2-2.2.8.103.jar                       | None                                     |
       | LCHIJA  | jeibees                           | 0.9.0.5                  | jeibees-0.9.0.5-mc1.12.2.jar                      | None                                     |
       | LCHIJA  | journeymap                        | 1.12.2-5.7.1             | journeymap-1.12.2-5.7.1.jar                       | None                                     |
       | LCHIJA  | jehc                              | 1.7.2                    | just-enough-harvestcraft-1.12.2-1.7.2.jar         | None                                     |
       | LCHIJA  | jecalculation                     | 1.12.2-3.2.5             | JustEnoughCalculation-1.12.2-3.2.5.jar            | None                                     |
       | LCHIJA  | jee                               | 1.0.8                    | JustEnoughEnergistics-1.12.2-1.0.8.jar            | None                                     |
       | LCHIJA  | jeresources                       | 0.9.2.60                 | JustEnoughResources-1.12.2-0.9.2.60.jar           | None                                     |
       | LCHIJA  | laggoggles                        | FAT-1.12.2-4.11-92       | LagGoggles-FAT-1.12.2-4.11-92.jar                 | None                                     |
       | LCHIJA  | letsencryptcraft                  | @VERSION@                | letsencryptcraft-1.10.2-1.2.0.jar                 | None                                     |
       | LCHIJA  | levelup2                          | ${version}               | levelup2-1.5.8.jar                                | None                                     |
       | LCHIJA  | littletiles                       | 1.5.0                    | LittleTiles_v1.5.0-pre327_mc1.12.2.jar            | None                                     |
       | LCHIJA  | lodsofemone                       | 0.1                      | LodsOfEmone-0.1.jar                               | None                                     |
       | LCHIJA  | login_shield                      | 1.12.2-6-g5654706        | Login_Shield-1.12.2-6-g5654706.jar                | None                                     |
       | LCHIJA  | lootcapacitortooltips             | 1.3                      | lootcapacitortooltips-1.3.jar                     | None                                     |
       | LCHIJA  | timecore                          | 1.0.1.1                  | TimeCore-1.12.2-1.0.1.1.jar                       | None                                     |
       | LCHIJA  | lootgames                         | 1.0.3.1                  | LootGames-1.12.2-1.0.3.1.jar                      | None                                     |
       | LCHIJA  | lostmagic                         | 1.0                      | lostmagic-1.0.2.jar                               | None                                     |
       | LCHIJA  | magicbees                         | 1.0                      | MagicBees-1.12.2-3.1.10.jar                       | None                                     |
       | LCHIJA  | malisiscore                       | 1.12.2-6.5.1-SNAPSHOT    | malisiscore-1.12.2-6.5.1.jar                      | None                                     |
       | LCHIJA  | malisisdoors                      | 1.12.2-7.3.0             | malisisdoors-1.12.2-7.3.0.jar                     | None                                     |
       | LCHIJA  | maxpotidext                       | 1.0.3                    | maxpotidext-1.0.3.jar                             | b851b8b7c7f4d8d0e910ff27618150ba80c026ec |
       | LCHIJA  | immersivetech                     | 1.8.94                   | MCTImmersiveTechnology-1.12.2-1.8.94.jar          | None                                     |
       | LCHIJA  | mcwroofs                          | 1.0.2                    | mcw-roofs-1.0.2-mc1.12.2.jar                      | None                                     |
       | LCHIJA  | mekanismgenerators                | 1.12.2-9.8.3.390         | MekanismGenerators-1.12.2-9.8.3.390.jar           | None                                     |
       | LCHIJA  | mekanismtools                     | 1.12.2-9.8.3.390         | MekanismTools-1.12.2-9.8.3.390.jar                | None                                     |
       | LCHIJA  | menumobs                          | 1.21                     | MenuMobs-1.12.2-1.21.jar                          | None                                     |
       | LCHIJA  | moartinkers                       | 0.6.0                    | moartinkers-0.6.0.jar                             | None                                     |
       | LCHIJA  | mob_grinding_utils                | 0.3.13                   | MobGrindingUtils-0.3.13.jar                       | None                                     |
       | LCHIJA  | numina                            | 1.12.2-1.0.38            | Numina-1.12.2-1.0.38.jar                          | None                                     |
       | LCHIJA  | powersuits                        | 1.12.2-1.0.46            | ModularPowersuits-1.12.2-1.0.46.jar               | None                                     |
       | LCHIJA  | moreoverlays                      | 1.15.1                   | moreoverlays-1.15.1-mc1.12.2.jar                  | None                                     |
       | LCHIJA  | guilib                            | $version                 | morepaintings-paintings-1.12.2-5.0.1.2.jar        | None                                     |
       | LCHIJA  | paintingselgui                    | $version                 | morepaintings-paintings-1.12.2-5.0.1.2.jar        | None                                     |
       | LCHIJA  | morepaintings                     | $version                 | morepaintings-paintings-1.12.2-5.0.1.2.jar        | None                                     |
       | LCHIJA  | morpheus                          | 1.12.2-3.5.106           | Morpheus-1.12.2-3.5.106.jar                       | None                                     |
       | LCHIJA  | mputils                           | 1.5.6                    | MPUtils-1.12.2-1.5.7.jar                          | None                                     |
       | LCHIJA  | multimob                          | 1.0.5                    | multimob-1.0.5.jar                                | None                                     |
       | LCHIJA  | naturesaura                       | 18.1                     | NaturesAura-18.1.jar                              | None                                     |
       | LCHIJA  | naturescompass                    | 1.8.5                    | NaturesCompass-1.12.2-1.8.5.jar                   | None                                     |
       | LCHIJA  | netherportalfix                   | 5.3.17                   | NetherPortalFix_1.12.1-5.3.17.jar                 | None                                     |
       | LCHIJA  | netherportalspread                | 5.1                      | netherportalspread_1.12.2-5.1.jar                 | None                                     |
       | LCHIJA  | recipehandler                     | 0.13                     | NoMoreRecipeConflict-0.13(1.12.2).jar             | None                                     |
       | LCHIJA  | norecipebook                      | 1.2.1                    | noRecipeBook_v1.2.2formc1.12.2.jar                | None                                     |
       | LCHIJA  | neid                              | 1.5.4.4                  | NotEnoughIDs-1.5.4.4.jar                          | None                                     |
       | LCHIJA  | oldjava                           | 1.1.11                   | OldJavaWarning-1.12.2-1.1.11.jar                  | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LCHIJA  | omlib                             | 3.1.4-249                | omlib-1.12.2-3.1.4-249.jar                        | None                                     |
       | LCHIJA  | openmods                          | 0.12.2                   | OpenModsLib-1.12.2-0.12.2.jar                     | d2a9a8e8440196e26a268d1f3ddc01b2e9c572a5 |
       | LCHIJA  | openblocks                        | 1.8.1                    | OpenBlocks-1.12.2-1.8.1.jar                       | d2a9a8e8440196e26a268d1f3ddc01b2e9c572a5 |
       | LCHIJA  | openmodularturrets                | 3.1.12-378               | openmodularturrets-1.12.2-3.1.12-378.jar          | None                                     |
       | LCHIJA  | oreexcavation                     | 1.4.150                  | OreExcavation-1.4.150.jar                         | None                                     |
       | LCHIJA  | packmode                          | 1.2.0                    | packmode-1.12.2-1.2.0.jar                         | None                                     |
       | LCHIJA  | packmodemenu                      | 1.0.4                    | PackModeMenu-1.0.4.jar                            | None                                     |
       | LCHIJA  | pamscookables                     | 1.1                      | pamscookables-1.1.jar                             | None                                     |
       | LCHIJA  | pigstep                           | 1.12                     | pigstep-1.12.jar                                  | None                                     |
       | LCHIJA  | placebo                           | 1.6.0                    | Placebo-1.12.2-1.6.0.jar                          | None                                     |
       | LCHIJA  | thermaldynamics                   | 2.5.6                    | ThermalDynamics-1.12.2-2.5.6.1-universal.jar      | None                                     |
       | LCHIJA  | simplyjetpacks                    | 2.2.14.67                | SimplyJetpacks2-1.12.2-2.2.14.67.jar              | None                                     |
       | LCHIJA  | plustic                           | 8.0.1.0                  | plustic-8.0.1.0.jar                               | None                                     |
       | LCHIJA  | portalgun                         | 7.1.0                    | PortalGun-1.12.2-7.1.0.jar                        | 4db5c2bd1b556f252a5b8b54b256d381b2a0a6b8 |
       | LCHIJA  | potioncore                        | 1.9_for_1.12.2           | PotionCore-1.9_for_1.12.2.jar                     | None                                     |
       | LCHIJA  | practicallogistics2               | 3.0.8                    | practicallogistics2-1.12.2-3.0.8-11.jar           | None                                     |
       | LCHIJA  | primitivemobs                     | 1.2.3a                   | primitivemobs-1.2.3a.jar                          | None                                     |
       | LCHIJA  | progressivebosses                 | 1.5.4                    | ProgressiveBosses-1.5.4-mc1.12.x.jar              | None                                     |
       | LCHIJA  | quarkoddities                     | 1                        | QuarkOddities-1.12.2.jar                          | None                                     |
       | LCHIJA  | rats                              | 3.2.14                   | rats-3.2.14-1.12.2.jar                            | None                                     |
       | LCHIJA  | reccomplex                        | 1.4.8.2                  | RecurrentComplex-1.4.8.2.jar                      | None                                     |
       | LCHIJA  | xreliquary                        | 1.12.2-1.3.4.796         | Reliquary-1.12.2-1.3.4.796.jar                    | None                                     |
       | LCHIJA  | resourceloader                    | 1.5.3                    | ResourceLoader-MC1.12.1-1.5.3.jar                 | d72e0dd57935b3e9476212aea0c0df352dd76291 |
       | LCHIJA  | rftoolsdim                        | 5.71                     | rftoolsdim-1.12-5.71.jar                          | None                                     |
       | LCHIJA  | roguelike                         | 2.3.2                    | RoguelikeDungeonsFnarEdition-1.12.2-2.3.2.jar     | None                                     |
       | LCHIJA  | savemystronghold                  | 1.12.2-1.0.0             | savemystronghold-1.12.2-1.0.0.jar                 | None                                     |
       | LCHIJA  | scannable                         | 1.6.3.26                 | Scannable-MC1.12.2-1.6.3.26.jar                   | None                                     |
       | LCHIJA  | signpost                          | 1.08.3                   | signpost-1.12.2-1.08.3.jar                        | None                                     |
       | LCHIJA  | storagenetwork                    | 1.8.1                    | SimpleStorageNetwork-1.12.2-1.8.1.jar             | 0e5cb559be7d03f3fc18b8cba547d663e25f28af |
       | LCHIJA  | simplycats                        | 1.12.2-0.0.3.1           | simplycats-1.12.2-0.0.3.1.jar                     | None                                     |
       | LCHIJA  | stevescarts                       | 2.4.32.137               | StevesCarts-1.12.2-2.4.32.137.jar                 | None                                     |
       | LCHIJA  | storagedrawers                    | 5.2.2                    | StorageDrawers-1.12.2-5.4.2.jar                   | None                                     |
       | LCHIJA  | storagedrawersextra               | @VERSION@                | StorageDrawersExtras-1.12-3.1.0.jar               | None                                     |
       | LCHIJA  | streams                           | 0.4.9                    | Streams-1.12-0.4.9.jar                            | None                                     |
       | LCHIJA  | stupidthings                      | 1.1.6                    | Stupid Things-1.12.2-1.1.6.jar                    | None                                     |
       | LCHIJA  | stygian                           | 1.0.4                    | stygian-1.0.4.jar                                 | None                                     |
       | LCHIJA  | taiga                             | 1.12.2-1.3.3             | taiga-1.12.2-1.3.4.jar                            | None                                     |
       | LCHIJA  | tfspellpack                       | 1.1.0                    | TFSpellPack-1.1.0-MC1.12.2.jar                    | None                                     |
       | LCHIJA  | thaumicaugmentation               | 1.12.2-2.0.13            | ThaumicAugmentation-1.12.2-2.0.13.jar             | 8f678591ba6f78d579e553a8aa94b4c4766cb13d |
       | LCHIJA  | thaumicjei                        | 1.6.0                    | ThaumicJEI-1.12.2-1.6.0-27.jar                    | None                                     |
       | LCHIJA  | thaumicperiphery                  | 0.3.1                    | thaumicperiphery-0.3.1.jar                        | None                                     |
       | LCHIJA  | beneath                           | 1.7.0                    | The Beneath-1.12.2-1.7.0.jar                      | 220f10d3a93b3ff5fbaa7434cc629d863d6751b9 |
       | LCHIJA  | theaurorian                       | 1.12.2-Release           | theaurorian-1.12.2-release-mar2321.jar            | None                                     |
       | LCHIJA  | thermalcultivation                | 0.3.6                    | ThermalCultivation-1.12.2-0.3.6.1-universal.jar   | None                                     |
       | LCHIJA  | thermalinnovation                 | 0.3.6                    | ThermalInnovation-1.12.2-0.3.6.1-universal.jar    | None                                     |
       | LCHIJA  | thesummoner                       | 1.0.1-beta               | thesummoner-1.0.1.jar                             | None                                     |
       | LCHIJA  | tinkersjei                        | 1.2                      | tinkersjei-1.2.jar                                | None                                     |
       | LCHIJA  | tinkertoolleveling                | 1.12.2-1.1.0.DEV.b23e769 | TinkerToolLeveling-1.12.2-1.1.0.jar               | None                                     |
       | LCHIJA  | tips                              | 1.0.9                    | Tips-1.12.2-1.0.9.jar                             | d476d1b22b218a10d845928d1665d45fce301b27 |
       | LCHIJA  | totemic                           | 1.12.2-0.11.6            | Totemic-1.12.2-0.11.6.jar                         | 21d11d7bf4d97b465382a1f95428029aac6daaea |
       | LCHIJA  | treasure2                         | 1.16.0                   | Treasure2-mc1.12.2-f14.23.5.2854-v1.16.0.jar      | None                                     |
       | LCHIJA  | treechop                          | 0.14.4                   | TreeChop-1.12.2-0.14.4.jar                        | None                                     |
       | LCHIJA  | vampiresneedumbrellas             | 1.4                      | VampiresNeedUmbrellas-1.12.2-1.5.jar              | None                                     |
       | LCHIJA  | vampirism                         | 1.6.2                    | Vampirism-1.12.2-1.6.2.jar                        | None                                     |
       | LCHIJA  | teamlapen-lib                     | 1.6.2                    | Vampirism-1.12.2-1.6.2.jar                        | None                                     |
       | LCHIJA  | vampirism_integrations            | vampirism_integrations   | VampirismIntegrations-1.12.2-1.3.0.jar            | None                                     |
       | LCHIJA  | vanillafix                        | 1.0.10-150               | VanillaFix-1.0.10-150.jar                         | None                                     |
       | LCHIJA  | villagenames                      | 4.1.5                    | VillageNames-1.12.2-4.1.5.jar                     | None                                     |
       | LCHIJA  | wailaharvestability               | 1.1.12                   | WailaHarvestability-mc1.12-1.1.12.jar             | None                                     |
       | LCHIJA  | wanionlib                         | 1.12.2-2.5               | WanionLib-1.12.2-2.5.jar                          | None                                     |
       | LCHIJA  | waystones                         | 4.1.0                    | Waystones_1.12.2-4.1.0.jar                        | None                                     |
       | LCHIJA  | wings                             | 1.1.6                    | wings-1.1.6-1.12.2.jar                            | None                                     |
       | LCHIJA  | mowzies_wings                     | 1.0.0                    | wings-1.1.6-1.12.2.jar                            | None                                     |
       | LCHIJA  | bauble_wings                      | 1.0.0                    | wings-1.1.6-1.12.2.jar                            | None                                     |
       | LCHIJA  | wct                               | 3.12.97                  | WirelessCraftingTerminal-1.12.2-3.12.97.jar       | 186bc454cd122c9c2f1aa4f95611254bcc543363 |
       | LCHIJA  | witherskelefix                    | 2.6.3                    | WitherSkeletonTweaks-1.12.2-2.6.3.jar             | None                                     |
       | LCHIJA  | wgblockreplacer                   | 2.2.0                    | WorldgenBlockReplacer-1.12.2-2.2.0.jar            | None                                     |
       | LCHIJA  | wrcbe                             | 2.3.2                    | WR-CBE-1.12.2-2.3.2.33-universal.jar              | f1850c39b2516232a2108a7bd84d1cb5df93b261 |
       | LCHIJA  | xnet                              | 1.8.2                    | xnet-1.12-1.8.2.jar                               | None                                     |
       | LCHIJA  | yabba                             | 1.1.2.54                 | YABBA-1.1.2.54.jar                                | None                                     |
       | LCHIJA  | ynot                              | 0.2.4                    | YNot-0.2.4.jar                                    | None                                     |
       | LCHIJA  | yoyos                             | 1.12.2-1.3.3.25          | yoyos_1.12.2-1.3.3.25.jar                         | None                                     |
       | LCHIJA  | zerocore                          | 1.12.2-0.1.2.9           | zerocore-1.12.2-0.1.2.9.jar                       | None                                     |
       | LCHIJA  | lemonlib                          | 1.3.0                    | lemonlib-1.12.2-1.3.0.jar                         | None                                     |
       | LCHIJA  | arcaneworld                       | 0.0.11                   | arcaneworld-1.12.2-0.0.11.jar                     | None                                     |
       | LCHIJA  | rf-capability-adapter             | 1.1.1                    | capabilityadapter-1.1.1.jar                       | None                                     |
       | LCHIJA  | structurize                       | 1.12.2-0.10.277-RELEASE  | structurize-1.12.2-0.10.277-RELEASE.jar           | None                                     |
       | LCHIJA  | minecolonies                      | 1.12.2-0.11.811-BETA     | minecolonies-1.12.2-0.11.811-BETA-universal.jar   | None                                     |
       | LCHIJA  | phosphor-lighting                 | 1.12.2-0.2.6             | phosphor-1.12.2-0.2.6+build50-universal.jar       | f0387d288626cc2d937daa504e74af570c52a2f1 |
       | LCHIJA  | reauth                            | 3.6.0                    | reauth-3.6.0.jar                                  | daba0ec4df71b6da841768c49fb873def208a1e3 |
       | LCHIJA  | solcarrot                         | 1.8.4                    | solcarrot-1.12.2-1.8.4.jar                        | None                                     |
       | LCHIJA  | techreborn_compat                 | 1.0.0                    | TechReborn-ModCompatibility-1.12.2-1.4.0.76.jar   | 8727a3141c8ec7f173b87aa78b9b9807867c4e6b |
       | LCHIJA  | thebetweenlands                   | 3.7.3                    | TheBetweenlands-3.7.3-universal.jar               | 38067d6878811efb38b6a045521cfd80b9b60b38 |
       | LCHIJA  | midnight                          | 0.3.5                    | themidnight-0.3.5.jar                             | None                                     |
       | LCHIJA  | armoryexpansion-conarm            | 1.4.2                    | armoryexpansion-1.4.2.jar                         | None                                     |
       | LCHIJA  | mysticallib                       | 1.12.2-1.10.0            | mysticallib-1.12.2-1.10.0.jar                     | None                                     |
       | LCHIJA  | teslacorelib_registries           | 1.0.17                   | tesla-core-lib-1.12.2-1.0.17.jar                  | None                                     |
       | LCHIJA  | tweakersconstructpostload         | 1.12.2-1.6.0             | tweakersconstruct-1.12.2-1.6.0.jar                | None                                     |
       | LCHIJA  | unidict                           | 1.12.2-3.0.7             | UniDict-1.12.2-3.0.7.jar                          | None                                     |
       | LCHIJA  | wrapup                            | 1.12-1.1.3               | WrapUp-1.12-1.1.3.jar                             | None                                     |
       | UD      | mdecore-core                      | 1.0                      | minecraft.jar                                     | None                                     |
       | UD      | mobends_wings                     | 1.0.0                    | wings-1.1.6-1.12.2.jar                            | None                                     |
  Loaded coremods (and transformers): wings (wings-1.1.6-1.12.2.jar)
                                        me.paulf.wings.server.asm.WingsRuntimePatcher
                                        me.paulf.wings.server.asm.mobends.WingsMoBendsRuntimePatcher
                                      IELoadingPlugin (ImmersiveEngineering-core-0.12-98.jar)
                                        blusunrize.immersiveengineering.common.asm.IEClassTransformer
                                      TransformerLoader (OpenComputers-MC1.12.2-1.7.5.192.jar)
                                        li.cil.oc.common.asm.ClassTransformer
                                      Thaumic Augmentation Core Plugin (ThaumicAugmentation-1.12.2-2.0.13.jar)
                                        thecodex6824.thaumicaugmentation.core.TATransformer
                                      MekanismCoremod (Mekanism-1.12.2-9.8.3.390.jar)
                                        mekanism.coremod.KeybindingMigrationHelper
                                      LittlePatchingLoader (LittleTiles_v1.5.0-pre327_mc1.12.2.jar)
                                        com.creativemd.littletiles.LittleTilesTransformer
                                      BewitchmentFMLLoadingPlugin (bewitchment-1.12.2-0.0.22.64.jar)
                                        
                                      Quark Plugin (Quark-r1.6-179.jar)
                                        vazkii.quark.base.asm.ClassTransformer
                                      AppleCore (AppleCore-mc1.12.2-3.4.0.jar)
                                        squeek.applecore.asm.TransformerModuleHandler
                                      ObfuscatePlugin (obfuscate-0.4.2-1.12.2.jar)
                                        com.mrcrayfish.obfuscate.asm.ObfuscateTransformer
                                      iceandfire (iceandfire-1.9.1-1.12.2.jar)
                                        com.github.alexthe666.iceandfire.patcher.IceAndFireRuntimePatcher
                                      Inventory Tweaks Coremod (InventoryTweaks-1.63.jar)
                                        invtweaks.forge.asm.ContainerTransformer
                                      EnderCorePlugin (EnderCore-1.12.2-0.5.76-core.jar)
                                        com.enderio.core.common.transform.EnderCoreTransformer
                                        com.enderio.core.common.transform.SimpleMixinPatcher
                                      PhosphorFMLLoadingPlugin (phosphor-1.12.2-0.2.6+build50-universal.jar)
                                        
                                      ratscore (rats-3.2.14-1.12.2.jar)
                                        com.github.alexthe666.rats.server.misc.RatsRuntimePatcher
                                      LevelUpCore (levelup2-1.5.8.jar)
                                        
                                      LoadingPlugin (ResourceLoader-MC1.12.1-1.5.3.jar)
                                        lumien.resourceloader.asm.ClassTransformer
                                      MalisisCorePlugin (malisiscore-1.12.2-6.5.1.jar)
                                        
                                      CoreMod (Aroma1997Core-1.12.2-2.0.0.2.b167.jar)
                                        
                                      LoadingPlugin (HardcoreDarkness-MC1.12.2-2.0.jar)
                                        lumien.hardcoredarkness.asm.ClassTransformer
                                      CreativePatchingLoader (CreativeCore_v1.10.47_mc1.12.2.jar)
                                        
                                      IvToolkit (IvToolkit-1.3.3-1.12.jar)
                                        
                                      LoadingPlugin (Reskillable-1.12.2-1.13.0.jar)
                                        codersafterdark.reskillable.base.asm.ClassTransformer
                                      ColorUtilityCorePlugin (ColorUtility-universal-1.0.4.jar)
                                        com.Axeryok.ColorUtility.ColorUtilityTransformer
                                      FutureMC (future-mc-1.12.2-0.2.6.1.jar)
                                        thedarkcolour.futuremc.asm.CoreTransformer
                                      HCASM (HammerLib-1.12.2-2.0.6.26.jar)
                                        com.zeitheron.hammercore.asm.HammerCoreTransformer
                                      LoadingPlugin (RandomThings-MC1.12.2-4.2.7.4.jar)
                                        lumien.randomthings.asm.ClassTransformer
                                      ErebusFix Mixin Loading Plugin (erebusfix-1.12.2-0.0.0.1.jar)
                                        
                                      RandomPatches (randompatches-1.12.2-1.22.1.10.jar)
                                        com.therandomlabs.randompatches.core.RPTransformer
                                      ForgelinPlugin (Forgelin-1.8.4.jar)
                                        
                                      midnight (themidnight-0.3.5.jar)
                                        com.mushroom.midnight.core.transformer.MidnightClassTransformer
                                      Do not report to Forge! (If you haven't disabled the FoamFix coremod, try disabling it in the config! Note that this bit of text will still appear.) (foamfix-0.10.14-1.12.2.jar)
                                        pl.asie.foamfix.coremod.FoamFixTransformer
                                      OpenModsCorePlugin (OpenModsLib-1.12.2-0.12.2.jar)
                                        openmods.core.OpenModsClassTransformer
                                      CorePlugin (ForgeEndertech-1.12.2-4.5.5.0-build.0561.jar)
                                        
                                      CTMCorePlugin (CTM-MC1.12.2-1.0.2.31.jar)
                                        team.chisel.ctm.client.asm.CTMTransformer
                                      FarseekCoreMod (Farseek-1.12-2.5.1.jar)
                                        farseek.core.FarseekClassTransformer
                                      TheBetweenlandsLoadingPlugin (TheBetweenlands-3.7.3-SNAPSHOT-20210322.082210-core.jar)
                                        thebetweenlands.core.TheBetweenlandsClassTransformer
                                      AdvancedRocketryPlugin (AdvancedRocketry-1.12.2-1.7.0-232-universal.jar)
                                        zmaster587.advancedRocketry.asm.ClassTransformer
                                      CharmLoadingPlugin (Charm-1.12.2-1.4.1.jar)
                                        svenhjol.charm.base.CharmClassTransformer
                                      Plugin (NotEnoughIDs-1.5.4.4.jar)
                                        ru.fewizz.neid.asm.Transformer
                                      llibrary (llibrary-core-1.0.11-1.12.2.jar)
                                        net.ilexiconn.llibrary.server.core.plugin.LLibraryTransformer
                                        net.ilexiconn.llibrary.server.core.patcher.LLibraryRuntimePatcher
                                      AstralCore (astralsorcery-1.12.2-1.10.27.jar)
                                        
                                      MDECore-Core (mdecore-1.12-1.1.jar)
                                        com.mattdahepic.mdecore.asm.TickrateTransformer
                                      VanillaFixLoadingPlugin (VanillaFix-1.0.10-150.jar)
                                        
                                      Max Potion ID Extender (maxpotidext-1.0.3.jar)
                                        zabi.minecraft.maxpotidext.MPIDTransformer
  GL info: ~~ERROR~~ RuntimeException: No OpenGL context found in the current thread.
  OpenModsLib class transformers: [llama_null_fix:FINISHED],[horse_base_null_fix:FINISHED],[pre_world_render_hook:FINISHED],[player_render_hook:FINISHED],[horse_null_fix:FINISHED]
  AE2 Version: stable rv6-stable-7 for Forge 14.23.5.2768
  Ender IO: No known problems detected.
            Authlib is : /C:/Users/24win/curseforge/minecraft/Install/libraries/com/mojang/authlib/1.5.25/authlib-1.5.25.jar
            
            !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
            !!!You are looking at the diagnostics information, not at the crash.       !!!
            !!!Scroll up until you see the line with '---- Minecraft Crash Report ----'!!!
            !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
  Pulsar/tconstruct loaded Pulses: - TinkerCommons (Enabled/Forced)
                                   - TinkerWorld (Enabled/Not Forced)
                                   - TinkerTools (Enabled/Not Forced)
                                   - TinkerHarvestTools (Enabled/Forced)
                                   - TinkerMeleeWeapons (Enabled/Forced)
                                   - TinkerRangedWeapons (Enabled/Forced)
                                   - TinkerModifiers (Enabled/Forced)
                                   - TinkerSmeltery (Enabled/Not Forced)
                                   - TinkerGadgets (Enabled/Not Forced)
                                   - TinkerOredict (Enabled/Forced)
                                   - TinkerIntegration (Enabled/Forced)
                                   - TinkerFluids (Enabled/Forced)
                                   - TinkerMaterials (Enabled/Forced)
                                   - TinkerModelRegister (Enabled/Forced)
                                   - chiselIntegration (Enabled/Not Forced)
                                   - chiselsandbitsIntegration (Enabled/Not Forced)
                                   - craftingtweaksIntegration (Enabled/Not Forced)
                                   - wailaIntegration (Enabled/Not Forced)
                                   - quarkIntegration (Enabled/Not Forced)
  HammerCore Debug Information: Dependent Mods:
                                -Thaumic Additions: Reconstructed (thaumadditions) @ 12.6.6
  List of loaded APIs: * actuallyadditionsapi (34) from ActuallyAdditions-1.12.2-r152.jar
                       * ae2wtlib|API (1.0.34) from AE2WTLib-1.12.2-1.0.34.jar
                       * AgriCraftAPI (1.0) from AgriCraft-2.12.0-1.12.0-a6.jar
                       * AppleCoreAPI (3.4.0) from AppleCore-mc1.12.2-3.4.0.jar
                       * appliedenergistics2|API (rv6) from appliedenergistics2-rv6-stable-7.jar
                       * AtumAPI (0.0.2) from Atum-1.12.2-2.0.20.jar
                       * Baubles|API (1.4.0.2) from Baubles-1.12-1.5.2.jar
                       * BetterWithModsAPI (Beta 0.6) from AppleSkin-mc1.12-1.0.14.jar
                       * BetweenlandsAPI (1.13.1) from TheBetweenlands-3.7.3-universal.jar
                       * bloodmagic-api (2.0.0) from BloodMagic-1.12.2-2.4.3-105.jar
                       * BotaniaAPI (89) from Bountiful Baubles-1.12.2-0.1.6.jar
                       * buildcraftapi_blocks (1.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_boards (2.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_core (2.2) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_crops (1.1) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_enums (1.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_events (2.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_facades (1.1) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_filler (5.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_fuels (2.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_gates (4.1) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_items (1.1) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_library (2.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_lists (1.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_power (1.3) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_recipes (3.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_robotics (3.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_statements (1.1) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_tiles (1.2) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_tools (1.0) from buildcraft-all-7.99.24.8.jar
                       * buildcraftapi_transport (5.0) from buildcraft-all-7.99.24.8.jar
                       * Chisel-API (0.0.1) from Chisel-MC1.12.2-1.0.2.45.jar
                       * ChiselAPI|Carving (0.0.1) from Chisel-MC1.12.2-1.0.2.45.jar
                       * ChiselsAndBitsAPI (14.25.0) from chiselsandbits-14.33.jar
                       * cofhapi (2.5.0) from CoFHCore-1.12.2-4.6.6.1-universal.jar
                       * commoncapabilities|api (0.0.1) from CommonCapabilities-1.12.2-2.4.8.jar
                       * cosmeticarmorreworked|api (1.0.0) from CosmeticArmorReworked-1.12.2-v5a.jar
                       * CraftingTweaks|API (4.1) from CraftingTweaks_1.12.2-8.1.9.jar
                       * ctm-api (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
                       * ctm-api-events (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
                       * ctm-api-models (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
                       * ctm-api-textures (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
                       * ctm-api-utils (0.1.0) from CTM-MC1.12.2-1.0.2.31.jar
                       * Culinary Construct API (1) from culinaryconstruct-1.3.4.jar
                       * DarknessLibAPI (1.1.0) from DarknessLib-1.12.2-1.1.0.jar
                       * DarknessLibAPI|Cap (1.1.0) from DarknessLib-1.12.2-1.1.0.jar
                       * DarknessLibAPI|Internal (1.1.0) from DarknessLib-1.12.2-1.1.0.jar
                       * enderioapi (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|addon (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|capacitor (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|conduits (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|farm (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|redstone (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|teleport (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|tools (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * enderioapi|upgrades (4.0.0) from EnderIO-1.12.2-5.3.70.jar
                       * farmingforblockheads|api (1.0) from FarmingForBlockheads_1.12.2-3.1.28.jar
                       * ForestryAPI|apiculture (5.0.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|arboriculture (4.3.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|book (5.8.1) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|circuits (3.1.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|climate (5.0.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|core (5.7.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|farming (5.8.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|food (1.1.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|fuels (3.0.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|genetics (5.7.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|gui (5.8.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|hives (4.1.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|lepidopterology (1.4.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|mail (3.1.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|modules (5.7.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|multiblock (3.0.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|recipes (5.4.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|storage (5.0.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForestryAPI|world (2.1.0) from forestry_1.12.2-5.8.2.422.jar
                       * ForgeEndertechAPI (1.0) from ForgeEndertech-1.12.2-4.5.5.0-build.0561.jar
                       * gendustryAPI (2.3.0) from gendustry-1.6.5.8-mc1.12.2.jar
                       * Guide-API|API (2.0.0) from Guide-API-1.12-2.1.8-63.jar
                       * iChunUtil API (1.2.0) from iChunUtil-1.12.2-7.2.2.jar
                       * ImmersiveEngineering|API (1.0) from ImmersiveEngineering-0.12-98.jar
                       * ImmersiveEngineering|ImmersiveFluxAPI (1.0) from ImmersiveEngineering-0.12-98.jar
                       * ImprovedBackpacks|API (1.2.0.3) from ImprovedBackpacks-1.12.2-1.5.0.0.jar
                       * industrialforegoingapi (5) from industrialforegoing-1.12.2-1.12.13-237.jar
                       * integrateddynamics|api (0.2.0) from IntegratedDynamics-1.12.2-1.1.11.jar
                       * jeresources|API (0.9.2.60) from JustEnoughResources-1.12.2-0.9.2.60.jar
                       * journeymap|client-api (1.4) from journeymap-1.12.2-5.7.1.jar
                       * journeymap|client-api-display (1.4) from journeymap-1.12.2-5.7.1.jar
                       * journeymap|client-api-event (1.4) from journeymap-1.12.2-5.7.1.jar
                       * journeymap|client-api-model (1.4) from journeymap-1.12.2-5.7.1.jar
                       * journeymap|client-api-util (1.4) from journeymap-1.12.2-5.7.1.jar
                       * JustEnoughItemsAPI (4.13.0) from jei_1.12.2-4.16.1.301.jar
                       * MekanismAPI|core (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
                       * MekanismAPI|energy (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
                       * MekanismAPI|gas (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
                       * MekanismAPI|infuse (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
                       * MekanismAPI|laser (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
                       * MekanismAPI|transmitter (9.8.1) from Mekanism-1.12.2-9.8.3.390.jar
                       * MekanismAPI|util (9.0.0) from Mekanism-1.12.2-9.8.3.390.jar
                       * minecolonies-api (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|achievements (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|blocks (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|blocks|decorative (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|blocks|huts (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|blocks|interfaces (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|blocks|types (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|client (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|client|render (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|client|render|modeltype (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|client|render|modeltype|registry (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|buildings (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|buildings|registry (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|buildings|views (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|buildings|workerbuildings (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|guardtype (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|guardtype|registry (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|jobs (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|jobs|registry (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|managers (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|managers|interfaces (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|permissions (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|data (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|factory (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|factory|standard (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|location (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|manager (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|request (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|requestable (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|requestable|crafting (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|requester (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|resolver (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|resolver|player (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|resolver|retrying (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|requestsystem|token (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|colony|workorders (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|compatibility (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|compatibility|candb (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|compatibility|dynamictrees (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|compatibility|gbook (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|compatibility|tinkers (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|configuration (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|crafting (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|creativetab (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|citizen (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|citizen|builder (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|citizen|guards (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|pathfinding (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|registry (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|statemachine (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|statemachine|basestatemachine (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|statemachine|states (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|statemachine|tickratestatemachine (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|ai|statemachine|transition (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|citizen (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|citizen|citizenhandlers (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|mobs (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|mobs|barbarians (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|mobs|pirates (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|mobs|util (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|pathfinding (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|entity|pathfinding|registry (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|inventory (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|inventory|api (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|items (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|network (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|sounds (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|tileentities (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|util (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-api|util|constants (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-blockout (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-blockout|controls (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * minecolonies-blockout|views (1.12.2-0.11.811-BETA) from minecolonies-1.12.2-0.11.811-BETA-universal.jar
                       * MouseTweaks|API (1.0) from MouseTweaks-2.10-mc1.12.2.jar
                       * naturesauraapi (9) from NaturesAura-18.1.jar
                       * openblocks|api (1.2) from OpenBlocks-1.12.2-1.8.1.jar
                       * opencomputersapi|component (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|core (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|driver (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|driver|item (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|event (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|filesystem (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|internal (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|machine (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|manual (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|network (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * opencomputersapi|prefab (7.0.0-alpha) from OpenComputers-MC1.12.2-1.7.5.192.jar
                       * PatchouliAPI (6) from Patchouli-1.0-23.6.jar
                       * practicallogistics2-api (3.1) from practicallogistics2-1.12.2-3.0.8-11.jar
                       * QuarkAPI (4) from Quark-r1.6-179.jar
                       * reborncoreAPI (3.19.5) from RebornCore-FORK-1.12.2-3.19.5-universal.jar
                       * reborncoreAPI|Power (3.19.5) from RebornCore-FORK-1.12.2-3.19.5-universal.jar
                       * reborncoreAPI|Recipe (3.19.5) from RebornCore-FORK-1.12.2-3.19.5-universal.jar
                       * reborncoreAPI|Tile (3.19.5) from RebornCore-FORK-1.12.2-3.19.5-universal.jar
                       * redstonefluxapi (2.1.1) from RedstoneFlux-1.12-2.1.1.1-universal.jar
                       * sonarapi (1.0.1) from sonarcore-1.12.2-5.0.19-20.jar
                       * stevescartsAPI (${version}) from StevesCarts-1.12.2-2.4.32.137.jar
                       * stevescartsAPI|FARMS (${version}) from StevesCarts-1.12.2-2.4.32.137.jar
                       * StorageDrawersAPI (2.1.0) from StorageDrawers-1.12.2-5.4.2.jar
                       * StorageDrawersAPI|event (2.1.0) from StorageDrawers-1.12.2-5.4.2.jar
                       * StorageDrawersAPI|registry (2.1.0) from StorageDrawers-1.12.2-5.4.2.jar
                       * StorageDrawersAPI|render (2.1.0) from StorageDrawers-1.12.2-5.4.2.jar
                       * StorageDrawersAPI|storage (2.1.0) from StorageDrawers-1.12.2-5.4.2.jar
                       * StorageDrawersAPI|storage-attribute (2.1.0) from StorageDrawers-1.12.2-5.4.2.jar
                       * team_reborn|Praescriptum (3.19.5) from RebornCore-FORK-1.12.2-3.19.5-universal.jar
                       * techrebornAPI (2.27.3.1084) from TechReborn-1.12.2-2.27.3.1084-universal.jar
                       * Thaumcraft|API (6.0.2) from Thaumcraft-1.12.2-6.1.BETA26.jar
                       * thaumicaugmentationapi (2.0.13) from ThaumicAugmentation-1.12.2-2.0.13.jar
                       * tombstone-api (1.0.8) from tombstone-4.1.2-1.12.2.jar
                       * tombstone-api-capability (1.0.8) from tombstone-4.1.2-1.12.2.jar
                       * tombstone-api-event (1.0.8) from tombstone-4.1.2-1.12.2.jar
                       * tombstone-api-magic (1.0.8) from tombstone-4.1.2-1.12.2.jar
                       * tombstone-api-recipe (1.0.8) from tombstone-4.1.2-1.12.2.jar
                       * totemic|API (1.12.2-7.1.0) from Totemic-1.12.2-0.11.6.jar
                       * VampirismAPI (1.4) from Vampirism-1.12.2-1.6.2.jar
                       * WailaAPI (1.3) from Hwyla-1.8.26-B41_1.12.2.jar
                       * wct|api (1.1) from WirelessCraftingTerminal-1.12.2-3.12.97.jar
                       * zerocore|API|multiblock (1.10.2-0.0.2) from zerocore-1.12.2-0.1.2.9.jar
                       * zerocore|API|multiblock|rectangular (1.10.2-0.0.2) from zerocore-1.12.2-0.1.2.9.jar
                       * zerocore|API|multiblock|tier (1.10.2-0.0.2) from zerocore-1.12.2-0.1.2.9.jar
                       * zerocore|API|multiblock|validation (1.10.2-0.0.2) from zerocore-1.12.2-0.1.2.9.jar
  Patchouli open book context: n/a
  RebornCore: Plugin Engine: 0
              RebornCore Version: 3.19.5
              Runtime Debofucsation 1
              Invalid fingerprint detected for RebornCore!
              RenderEngine: 0
  AE2 Integration: IC2:OFF, RC:OFF, MFR:OFF, Waila:ON, InvTweaks:ON, JEI:ON, Mekanism:ON, OpenComputers:ON, THE_ONE_PROBE:OFF, TESLA:OFF, CRAFTTWEAKER:ON
  Suspected Mods: EnderStorage (enderstorage)
  Profiler Position: N/A (disabled)
  Player Count: 0 / 8; []
  Type: Integrated Server (map_client.txt)
  Is Modded: Definitely; Client brand changed to 'fml,forge'

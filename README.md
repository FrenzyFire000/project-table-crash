# project-table-crash

---- Minecraft Crash Report ----
// But it works on my machine.

Time: 11/4/15 10:04 AM
Description: Rendering screen

java.lang.IndexOutOfBoundsException
	at java.nio.Buffer.checkIndex(Unknown Source)
	at java.nio.DirectByteBuffer.get(Unknown Source)
	at org.lwjgl.input.Keyboard.isKeyDown(Keyboard.java:407)
	at uk.co.qmunity.lib.proxy.ClientProxy.isSneakingInGui(ClientProxy.java:46)
	at uk.co.qmunity.lib.client.gui.GuiContainerBase.func_73863_a(GuiContainerBase.java:148)
	at net.minecraft.client.renderer.EntityRenderer.func_78480_b(EntityRenderer.java:1061)
	at net.minecraft.client.Minecraft.func_71411_J(Minecraft.java:1001)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:898)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at java.nio.Buffer.checkIndex(Unknown Source)
	at java.nio.DirectByteBuffer.get(Unknown Source)
	at org.lwjgl.input.Keyboard.isKeyDown(Keyboard.java:407)
	at uk.co.qmunity.lib.proxy.ClientProxy.isSneakingInGui(ClientProxy.java:46)
	at uk.co.qmunity.lib.client.gui.GuiContainerBase.func_73863_a(GuiContainerBase.java:148)

-- Screen render details --
Details:
	Screen name: com.bluepowermod.client.gui.GuiProjectTable
	Mouse location: Scaled: (240, 134). Absolute: (960, 540)
	Screen size: Scaled: (480, 270). Absolute: (1920, 1080). Scale factor of 4

-- Affected level --
Details:
	Level name: MpServer
	All players: 1 total; [EntityClientPlayerMP['FrenzyFire000'/368, l='MpServer', x=-639.67, y=5.62, z=-938.08]]
	Chunk stats: MultiplayerChunkCache: 121, 121
	Level seed: 0
	Level generator: ID 01 - flat, ver 0. Features enabled: false
	Level generator options: 
	Level spawn location: World: (-639,4,-960), Chunk: (at 1,0,0 in -40,-60; contains blocks -640,0,-960 to -625,255,-945), Region: (-2,-2; contains chunks -64,-64 to -33,-33, blocks -1024,0,-1024 to -513,255,-513)
	Level time: 6446 game time, 55198 day time
	Level dimension: 0
	Level storage version: 0x00000 - Unknown?
	Level weather: Rain time: 0 (now: false), thunder time: 0 (now: false)
	Level game mode: Game mode: creative (ID 1). Hardcore: false. Cheats: false
	Forced entities: 125 total; [EntityPig['Pig'/256, l='MpServer', x=-559.19, y=4.00, z=-899.25], EntityPig['Pig'/257, l='MpServer', x=-563.50, y=4.00, z=-893.50], EntitySlime['Slime'/289303, l='MpServer', x=-600.09, y=4.00, z=-973.84], EntitySlime['Slime'/288542, l='MpServer', x=-605.08, y=5.00, z=-1000.09], EntitySlime['Slime'/217633, l='MpServer', x=-604.35, y=4.47, z=-982.23], EntityItem['item.item.bone'/50468, l='MpServer', x=-622.34, y=3.13, z=-937.84], EntitySlime['Slime'/249387, l='MpServer', x=-594.88, y=5.01, z=-971.68], EntityCreeper['Creeper'/553, l='MpServer', x=-708.50, y=4.00, z=-865.50], EntitySpider['Spider'/558, l='MpServer', x=-708.59, y=4.00, z=-992.41], EntitySlime['Slime'/239665, l='MpServer', x=-649.53, y=4.00, z=-896.41], EntitySpider['Spider'/567, l='MpServer', x=-613.50, y=4.00, z=-866.50], EntitySlime['Slime'/33087, l='MpServer', x=-591.33, y=4.00, z=-870.88], EntitySlime['Slime'/165696, l='MpServer', x=-665.46, y=4.18, z=-898.25], EntitySlime['Slime'/257351, l='MpServer', x=-613.30, y=4.99, z=-996.46], EntitySlime['Slime'/193605, l='MpServer', x=-694.13, y=4.00, z=-893.44], EntitySlime['Slime'/12616, l='MpServer', x=-642.73, y=5.02, z=-976.82], EntitySlime['Slime'/110666, l='MpServer', x=-612.64, y=4.00, z=-919.60], EntitySlime['Slime'/147785, l='MpServer', x=-695.16, y=4.81, z=-871.75], EntitySlime['Slime'/37463, l='MpServer', x=-594.23, y=4.47, z=-968.08], EntityItem['item.item.rottenFlesh'/45914, l='MpServer', x=-606.06, y=4.13, z=-946.84], EntityCow['Cow'/94, l='MpServer', x=-714.09, y=4.00, z=-901.94], EntitySlime['Slime'/130657, l='MpServer', x=-674.03, y=4.00, z=-931.22], EntityCow['Cow'/100, l='MpServer', x=-707.03, y=4.00, z=-997.94], EntityCow['Cow'/101, l='MpServer', x=-704.28, y=4.00, z=-946.41], EntitySlime['Slime'/196709, l='MpServer', x=-641.47, y=4.00, z=-896.59], EntitySlime['Slime'/358, l='MpServer', x=-566.73, y=4.82, z=-979.74], EntityCreeper['Creeper'/616, l='MpServer', x=-567.22, y=4.00, z=-904.78], EntityCow['Cow'/105, l='MpServer', x=-707.50, y=4.00, z=-891.78], EntityCow['Cow'/106, l='MpServer', x=-707.50, y=4.00, z=-890.19], EntityCow['Cow'/107, l='MpServer', x=-708.50, y=4.00, z=-895.50], EntityPig['Pig'/108, l='MpServer', x=-705.38, y=4.00, z=-891.59], EntityCow['Cow'/111, l='MpServer', x=-700.47, y=4.00, z=-1008.44], EntityCow['Cow'/112, l='MpServer', x=-695.50, y=4.00, z=-993.50], EntityClientPlayerMP['FrenzyFire000'/368, l='MpServer', x=-639.67, y=5.62, z=-938.08], EntityCow['Cow'/113, l='MpServer', x=-700.50, y=4.00, z=-992.50], EntityChicken['Chicken'/114, l='MpServer', x=-697.50, y=4.00, z=-992.50], EntityChicken['Chicken'/115, l='MpServer', x=-702.41, y=4.00, z=-996.53], EntityChicken['Chicken'/116, l='MpServer', x=-691.56, y=4.00, z=-988.56], EntityCow['Cow'/117, l='MpServer', x=-710.25, y=4.00, z=-991.44], EntityCow['Cow'/118, l='MpServer', x=-700.34, y=4.00, z=-1002.53], EntityCow['Cow'/119, l='MpServer', x=-700.81, y=4.00, z=-1000.50], EntityCow['Cow'/120, l='MpServer', x=-702.50, y=4.00, z=-989.50], EntityChicken['Chicken'/121, l='MpServer', x=-690.59, y=4.00, z=-983.53], EntityChicken['Chicken'/122, l='MpServer', x=-698.91, y=4.00, z=-961.09], EntityChicken['Chicken'/124, l='MpServer', x=-708.34, y=4.00, z=-953.41], EntityChicken['Chicken'/125, l='MpServer', x=-697.69, y=4.00, z=-954.47], EntityChicken['Chicken'/126, l='MpServer', x=-701.41, y=4.00, z=-953.44], EntityHorse['Horse'/127, l='MpServer', x=-702.75, y=4.00, z=-948.88], EntityHorse['Horse'/128, l='MpServer', x=-701.88, y=4.00, z=-954.72], EntityCow['Cow'/129, l='MpServer', x=-700.69, y=4.00, z=-948.78], EntityCow['Cow'/130, l='MpServer', x=-698.22, y=4.00, z=-958.75], EntitySlime['Slime'/129411, l='MpServer', x=-643.88, y=4.69, z=-981.12], EntityHorse['Horse'/131, l='MpServer', x=-697.63, y=4.00, z=-943.84], EntitySlime['Slime'/65666, l='MpServer', x=-697.21, y=4.00, z=-861.58], EntityHorse['Horse'/132, l='MpServer', x=-699.84, y=4.00, z=-942.66], EntityPig['Pig'/133, l='MpServer', x=-699.28, y=4.00, z=-892.09], EntityPig['Pig'/134, l='MpServer', x=-692.63, y=4.00, z=-894.03], EntityPig['Pig'/135, l='MpServer', x=-696.84, y=4.00, z=-889.09], EntityPig['Pig'/136, l='MpServer', x=-703.00, y=4.00, z=-876.16], EntityPig['Pig'/137, l='MpServer', x=-697.50, y=4.00, z=-886.50], EntityPig['Pig'/138, l='MpServer', x=-702.28, y=4.00, z=-881.53], EntityPig['Pig'/139, l='MpServer', x=-690.47, y=4.00, z=-874.50], EntityChicken['Chicken'/148, l='MpServer', x=-674.53, y=4.00, z=-971.59], EntityChicken['Chicken'/149, l='MpServer', x=-682.13, y=4.00, z=-978.63], EntityChicken['Chicken'/150, l='MpServer', x=-676.44, y=4.00, z=-978.47], EntityHorse['Horse'/151, l='MpServer', x=-681.41, y=4.00, z=-977.22], EntityHorse['Horse'/152, l='MpServer', x=-683.00, y=4.00, z=-972.50], EntityItem['item.item.arrow'/50072, l='MpServer', x=-605.78, y=4.13, z=-943.25], EntityPig['Pig'/153, l='MpServer', x=-679.78, y=4.00, z=-972.16], EntityPig['Pig'/154, l='MpServer', x=-670.06, y=4.00, z=-968.03], EntityItem['item.item.bone'/50074, l='MpServer', x=-606.56, y=4.13, z=-943.44], EntityChicken['Chicken'/155, l='MpServer', x=-680.63, y=4.00, z=-972.44], EntityHorse['Horse'/156, l='MpServer', x=-679.94, y=4.00, z=-975.59], EntityItem['item.item.bone'/60061, l='MpServer', x=-607.00, y=4.13, z=-880.25], EntitySlime['Slime'/239013, l='MpServer', x=-638.59, y=4.00, z=-866.63], EntityPig['Pig'/167, l='MpServer', x=-671.22, y=4.00, z=-966.88], EntityCow['Cow'/168, l='MpServer', x=-662.47, y=4.00, z=-914.25], EntityCow['Cow'/169, l='MpServer', x=-668.81, y=4.00, z=-920.16], EntityCow['Cow'/170, l='MpServer', x=-666.59, y=4.00, z=-917.25], EntitySlime['Slime'/60842, l='MpServer', x=-607.88, y=4.00, z=-943.63], EntityCow['Cow'/171, l='MpServer', x=-677.75, y=4.00, z=-923.66], EntityCow['Cow'/172, l='MpServer', x=-669.75, y=4.00, z=-922.66], EntityCow['Cow'/173, l='MpServer', x=-659.69, y=4.00, z=-909.22], EntitySlime['Slime'/255918, l='MpServer', x=-608.45, y=4.85, z=-938.45], EntityCow['Cow'/174, l='MpServer', x=-668.06, y=4.00, z=-917.88], EntityCow['Cow'/175, l='MpServer', x=-667.75, y=4.00, z=-914.81], EntityCow['Cow'/176, l='MpServer', x=-663.53, y=4.00, z=-913.03], EntityCow['Cow'/178, l='MpServer', x=-662.84, y=4.00, z=-901.13], EntityCow['Cow'/179, l='MpServer', x=-661.09, y=4.00, z=-904.88], EntitySlime['Slime'/96955, l='MpServer', x=-620.42, y=4.18, z=-897.08], EntityCow['Cow'/190, l='MpServer', x=-649.72, y=4.00, z=-919.28], EntitySlime['Slime'/281284, l='MpServer', x=-677.68, y=5.01, z=-965.58], EntityItem['item.item.arrow'/49096, l='MpServer', x=-666.66, y=4.13, z=-964.91], EntityItem['item.item.bone'/49098, l='MpServer', x=-667.34, y=4.13, z=-965.56], EntitySlime['Slime'/306120, l='MpServer', x=-675.94, y=4.00, z=-986.84], EntityBat['Bat'/209, l='MpServer', x=-584.59, y=6.57, z=-861.85], EntityBat['Bat'/210, l='MpServer', x=-611.01, y=5.48, z=-878.04], EntitySlime['Slime'/120787, l='MpServer', x=-650.76, y=4.00, z=-981.35], EntitySlime['Slime'/165335, l='MpServer', x=-602.02, y=4.00, z=-982.92], EntitySlime['Slime'/312530, l='MpServer', x=-602.71, y=4.00, z=-1001.68], EntitySlime['Slime'/253656, l='MpServer', x=-715.10, y=5.01, z=-910.95], EntitySlime['Slime'/237533, l='MpServer', x=-601.37, y=4.88, z=-869.73], EntitySlime['Slime'/309474, l='MpServer', x=-684.53, y=4.00, z=-970.15], EntitySheep['Sheep'/237, l='MpServer', x=-567.97, y=4.00, z=-962.09], EntitySheep['Sheep'/238, l='MpServer', x=-564.50, y=4.00, z=-961.50], EntityChicken['Chicken'/239, l='MpServer', x=-560.41, y=4.00, z=-973.47], EntityPig['Pig'/240, l='MpServer', x=-570.22, y=4.00, z=-961.94], EntitySheep['Sheep'/241, l='MpServer', x=-570.47, y=4.00, z=-952.91], EntitySheep['Sheep'/242, l='MpServer', x=-565.69, y=4.00, z=-952.66], EntitySheep['Sheep'/243, l='MpServer', x=-564.50, y=4.00, z=-957.50], EntitySlime['Slime'/44275, l='MpServer', x=-689.49, y=4.00, z=-910.60], EntitySheep['Sheep'/244, l='MpServer', x=-566.50, y=4.00, z=-959.22], EntitySheep['Sheep'/245, l='MpServer', x=-564.97, y=4.00, z=-959.50], EntitySlime['Slime'/128500, l='MpServer', x=-698.16, y=4.14, z=-933.56], EntityPig['Pig'/246, l='MpServer', x=-567.81, y=4.00, z=-955.38], EntitySlime['Slime'/69879, l='MpServer', x=-651.12, y=4.32, z=-1015.70], EntityPig['Pig'/247, l='MpServer', x=-561.53, y=4.00, z=-957.19], EntityPig['Pig'/248, l='MpServer', x=-568.47, y=4.00, z=-903.47], EntityPig['Pig'/249, l='MpServer', x=-566.66, y=4.00, z=-903.16], EntityPig['Pig'/250, l='MpServer', x=-567.13, y=4.00, z=-898.59], EntityHorse['Horse'/251, l='MpServer', x=-571.50, y=4.00, z=-902.50], EntityHorse['Horse'/252, l='MpServer', x=-569.94, y=4.00, z=-902.94], EntityPig['Pig'/253, l='MpServer', x=-562.06, y=4.00, z=-895.88], EntityPig['Pig'/254, l='MpServer', x=-559.69, y=4.00, z=-897.28], EntityPig['Pig'/255, l='MpServer', x=-569.13, y=4.00, z=-888.97]]
	Retry entities: 0 total; []
	Server brand: fml,forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.WorldClient.func_72914_a(WorldClient.java:373)
	at net.minecraft.client.Minecraft.func_71396_d(Minecraft.java:2444)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:919)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_66, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 4740588240 bytes (4520 MB) / 5470420992 bytes (5217 MB) up to 7516192768 bytes (7168 MB)
	JVM Flags: 4 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx7168m -XX:+UseG1GC -XX:MaxGCPauseMillis=4
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP v9.05 FML v7.10.99.99 Minecraft Forge 10.13.4.1492 73 mods loaded, 73 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UCHIJAAAA	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) 
	UCHIJAAAA	FML{7.10.99.99} [Forge Mod Loader] (modpack.jar) 
	UCHIJAAAA	Forge{10.13.4.1492} [Minecraft Forge] (modpack.jar) 
	UCHIJAAAA	CodeChickenCore{1.0.6.41} [CodeChicken Core] (minecraft.jar) 
	UCHIJAAAA	NotEnoughItems{1.0.4.102} [Not Enough Items] (NotEnoughItems-1.7.10-1.0.4.102-universal.jar) 
	UCHIJAAAA	<CoFH ASM>{000} [CoFH ASM] (minecraft.jar) 
	UCHIJAAAA	mcdiscord{2.0.0} [MC Discord] (minecraft.jar) 
	UCHIJAAAA	CoFHCore{1.7.10R3.0.3} [CoFH Core] (CoFHCore-[1.7.10]3.0.3-303 (1).jar) 
	UCHIJAAAA	BuildCraft|Core{7.1.10} [BuildCraft] (buildcraft-7.1.10.jar) 
	UCHIJAAAA	BuildCraft|Transport{7.1.10} [BC Transport] (buildcraft-7.1.10.jar) 
	UCHIJAAAA	BuildCraft|Silicon{7.1.10} [BC Silicon] (buildcraft-7.1.10.jar) 
	UCHIJAAAA	BuildCraft|Factory{7.1.10} [BC Factory] (buildcraft-7.1.10.jar) 
	UCHIJAAAA	ComputerCraft{1.74} [ComputerCraft] (ComputerCraftPlusComputerCraftEdu1.74.jar) 
	UCHIJAAAA	IC2{2.2.999} [Industrial Craft Classic] (IC2.Classic.Version.1.1.2.1.jar) 
	UCHIJAAAA	Forestry{3.6.11.2} [Forestry for Minecraft] (forestry_1.7.10-3.6.11.2.jar) 
	UCHIJAAAA	LogisticsPipes{0.9.3.54} [Logistics Pipes] (logisticspipes-0.9.3.54.jar) 
	UCHIJAAAA	additionalpipes{4.7.0} [Additional Pipes] (additionalpipes-4.7.0.jar) 
	UCHIJAAAA	asielib{0.4.2} [asielib] (AsieLib-1.7.10-0.4.2.jar) 
	UCHIJAAAA	bdlib{1.9.3.107} [BD Lib] (bdlib-1.9.3.107-mc1.7.10.jar) 
	UCHIJAAAA	BigReactors{0.4.3A} [Big Reactors] (BigReactors-0.4.3A.jar) 
	UCHIJAAAA	qmunitylib{1.0} [QmunityLib] (QmunityLib-1.7.10-0.1.114-universal.jar) 
	UCHIJAAAA	bluepower{0.2.962} [Blue Power] (BluePower-1.7.10-0.2.962-universal.jar) 
	UCHIJAAAA	BuildCraft|Builders{7.1.10} [BC Builders] (buildcraft-7.1.10.jar) 
	UCHIJAAAA	BuildCraft|Energy{7.1.10} [BC Energy] (buildcraft-7.1.10.jar) 
	UCHIJAAAA	BuildCraft|Robotics{7.1.10} [BC Robotics] (buildcraft-7.1.10.jar) 
	UCHIJAAAA	BuildCraft|Compat{7.1.1} [BuildCraft Compat] (buildcraft-compat-7.1.1.jar) 
	UCHIJAAAA	CarpentersBlocks{3.3.7} [Carpenter's Blocks] (Carpenter's Blocks v3.3.7 - MC 1.7.10.jar) 
	UCHIJAAAA	ChickenChunks{1.3.4.19} [ChickenChunks] (ChickenChunks-1.7.10-1.3.4.19-universal.jar) 
	UCHIJAAAA	ComputerCraftEdu{1.74} [ComputerCraftEdu] (ComputerCraftPlusComputerCraftEdu1.74.jar) 
	UCHIJAAAA	Railcraft{9.7.0.0} [Railcraft] (Railcraft_1.7.10-9.7.0.0.jar) 
	UCHIJAAAA	Waila{1.5.10} [Waila] (Waila-1.5.10_1.7.10.jar) 
	UCHIJAAAA	computronics{1.5.7} [Computronics] (Computronics-1.7.10-1.5.7.jar) 
	UCHIJAAAA	defaultkeys{1.0.24} [Default Keyconfig] (defaultkeys-mc1.7.10-1.0.24.jar) 
	UCHIJAAAA	EnderStorage{1.4.7.36} [EnderStorage] (EnderStorage-1.7.10-1.4.7.36-universal.jar) 
	UCHIJAAAA	eng_toolbox{1.2.3.0} [Engineer's Toolbox] (EngineersToolbox-1.2.3.0-BETA.jar) 
	UCHIJAAAA	ForgeMultipart{1.2.0.344} [Forge Multipart] (ForgeMultipart-1.7.10-1.2.0.344-universal.jar) 
	UCHIJAAAA	McMultipart{1.2.0.344} [Minecraft Multipart Plugin] (ForgeMultipart-1.7.10-1.2.0.344-universal.jar) 
	UCHIJAAAA	gendustry{1.6.1.126} [GenDustry] (gendustry-1.6.1.126-mc1.7.10.jar) 
	UCHIJAAAA	IC2-Classic-Spmod{0.0.0.0} [IC2 Classic Detection Helper] (IC2.Classic.Version.1.1.2.1.jar) 
	UCHIJAAAA	IC2NuclearControl{2.3.0a-Butt} [Nuclear Control 2] (IC2NuclearControl-2.3.0a-Butt.jar) 
	UCHIJAAAA	ImmibisCore{59.1.2} [Immibis Core] (immibis-core-59.1.2.jar) 
	UCHIJAAAA	ImmibisPeripherals{59.0.2} [Immibis's Peripherals] (immibis-peripherals-59.0.2.jar) 
	UCHIJAAAA	inventorytweaks{1.59-dev-156-af3bc68} [Inventory Tweaks] (InventoryTweaks-1.59-dev-156.jar) 
	UCHIJAAAA	IronChest{6.0.60.741} [Iron Chest] (Ironchest-1.7.10-6.0.60.741-universal.jar) 
	UCHIJAAAA	itlt{0.0.8} [It's the little things] (itlt-1.7.10-0.0.8.jar) 
	UCHIJAAAA	JABBA{1.2.1} [JABBA] (Jabba-1.2.1a_1.7.10.jar) 
	UCHIJAAAA	MapWriter{2.1.8} [MapWriter] (MapWriter-1.7.10-2.1.10.jar) 
	UCHIJAAAA	MineTweaker3{3.0.10} [MineTweaker 3] (MineTweaker3-1.7.10-3.0.10.jar) 
	UCHIJAAAA	modtweaker2{0.9.2} [Mod Tweaker 2] (ModTweaker2-0.9.3.jar) 
	UCHIJAAAA	numina{0.4.0.131} [Numina] (Numina-0.4.0.131.jar) 
	UCHIJAAAA	powersuits{0.11.0.283} [MachineMuse's Modular Powersuits] (ModularPowersuits-0.11.0.283.jar) 
	UCHIJAAAA	NEIAddons{1.12.11.36} [NEI Addons] (neiaddons-1.12.11.36-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|Developer{1.12.11.36} [NEI Addons: Developer Tools] (neiaddons-1.12.11.36-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|AppEng{1.12.11.36} [NEI Addons: Applied Energistics 2] (neiaddons-1.12.11.36-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|Botany{1.12.11.36} [NEI Addons: Botany] (neiaddons-1.12.11.36-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|Forestry{1.12.11.36} [NEI Addons: Forestry] (neiaddons-1.12.11.36-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|CraftingTables{1.12.11.36} [NEI Addons: Crafting Tables] (neiaddons-1.12.11.36-mc1.7.10.jar) 
	UCHIJAAAA	NEIAddons|ExNihilo{1.12.11.36} [NEI Addons: Ex Nihilo] (neiaddons-1.12.11.36-mc1.7.10.jar) 
	UCHIJAAAA	neiintegration{1.0.12} [NEI Integration] (NEIIntegration-MC1.7.10-1.0.12.jar) 
	UCHIJAAAA	NetherOres{1.7.10R2.3.0} [Nether Ores] (NetherOres-[1.7.10]2.3.0-12.jar) 
	UCHIJAAAA	OCS{1.7.5} [OpenCCSensors] (openccsensors-1.7.5.jar) 
	UCHIJAAAA	planetguyLib{1.9} [planetguyLib] (PlanetguyLib-1.9.1.jar) 
	UCHIJAAAA	PowerConverters3{1.7.10-2.10} [Power Converters 3] (PowerConverters-1.7.10-2.10.jar) 
	UCHIJAAAA	ProjectE{1.7.10-PE1.9.3} [ProjectE] (ProjectE-1.7.10-PE1.9.3h.jar) 
	UCHIJAAAA	quiverchevsky{b100} [QuiverBow] (QuiverBow_1.7.10_b100.zip) 
	UCHIJAAAA	RedstoneArsenal{1.7.10R1.1.1} [Redstone Arsenal] (RedstoneArsenal-[1.7.10]1.1.1-89.jar) 
	UCHIJAAAA	JAKJ_RedstoneInMotion{2.8.6} [Remain In Motion] (RemainInMotion-2.8.6.jar) 
	UCHIJAAAA	SolarFlux{1.7.10-0.8b} [Solar Flux] (SolarFlux-1.7.10-0.8b.jar) 
	UCHIJAAAA	Tubestuff{59.0.4} [Tubestuff] (tubestuff-59.0.4.jar) 
	UCHIJAAAA	WailaHarvestability{1.1.2} [Waila Harvestability] (WailaHarvestability-mc1.7.x-1.1.2.jar) 
	UCHIJAAAA	zettaindustries{1.1} [Zetta Industries] (zettaindustries-1.1-97.jar) 
	UCHIJAAAA	aobd{2.8.4} [Another One Bites The Dust] (AOBD-2.8.4.jar) 
	UCHIJAAAA	ForgeMicroblock{1.2.0.344} [Forge Microblocks] (ForgeMultipart-1.7.10-1.2.0.344-universal.jar) 
	CoFHCore: -[1.7.10]3.0.3-303
	NetherOres: -[1.7.10]2.3.0-12
	RedstoneArsenal: -[1.7.10]1.1.1-89
	List of loaded APIs: 
		* apAPI (2) from additionalpipes-4.7.0.jar
		* asielibAPI (1.1) from AsieLib-1.7.10-0.4.2.jar
		* asielibAPI|chat (1.0) from AsieLib-1.7.10-0.4.2.jar
		* asielibAPI|tile (1.0) from AsieLib-1.7.10-0.4.2.jar
		* asielibAPI|tool (1.1) from AsieLib-1.7.10-0.4.2.jar
		* bluepowerAPI (1.0) from BluePower-1.7.10-0.2.962-universal.jar
		* BuildCraftAPI|blocks (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|blueprints (1.5) from buildcraft-7.1.10.jar
		* BuildCraftAPI|boards (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|core (1.4) from Railcraft_1.7.10-9.7.0.0.jar
		* BuildCraftAPI|crops (1.1) from buildcraft-7.1.10.jar
		* BuildCraftAPI|events (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|facades (1.1) from buildcraft-7.1.10.jar
		* BuildCraftAPI|filler (4.0) from buildcraft-7.1.10.jar
		* BuildCraftAPI|fuels (2.0) from buildcraft-7.1.10.jar
		* BuildCraftAPI|gates (4.1) from buildcraft-7.1.10.jar
		* BuildCraftAPI|items (1.1) from buildcraft-7.1.10.jar
		* BuildCraftAPI|library (1.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|lists (1.0) from buildcraft-7.1.10.jar
		* BuildCraftAPI|power (1.3) from buildcraft-7.1.10.jar
		* BuildCraftAPI|recipes (3.0) from buildcraft-7.1.10.jar
		* BuildCraftAPI|robotics (1.2) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|statements (1.1) from buildcraft-7.1.10.jar
		* BuildCraftAPI|tablet (1.0) from buildcraft-7.1.10.jar
		* BuildCraftAPI|tiles (1.2) from EngineersToolbox-1.2.3.0-BETA.jar
		* BuildCraftAPI|tools (1.0) from buildcraft-7.1.10.jar
		* BuildCraftAPI|transport (4.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* CarpentersBlocks|API (3.3.7) from Carpenter's Blocks v3.3.7 - MC 1.7.10.jar
		* CoFHAPI (1.7.10R1.0.2) from forestry_1.7.10-3.6.11.2.jar
		* CoFHAPI|block (1.7.10R1.0.12) from EngineersToolbox-1.2.3.0-BETA.jar
		* CoFHAPI|core (1.7.10R1.0.13) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHAPI|energy (1.7.10R1.0.2) from forestry_1.7.10-3.6.11.2.jar
		* CoFHAPI|fluid (1.7.10R1.0.12) from EngineersToolbox-1.2.3.0-BETA.jar
		* CoFHAPI|inventory (1.7.10R1.0.1) from buildcraft-compat-7.1.1.jar
		* CoFHAPI|item (1.7.10R1.0.12) from EngineersToolbox-1.2.3.0-BETA.jar
		* CoFHAPI|modhelpers (1.7.10R1.0.13) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHAPI|tileentity (1.7.10R1.0.12) from EngineersToolbox-1.2.3.0-BETA.jar
		* CoFHAPI|transport (1.7.10R1.0.1) from buildcraft-compat-7.1.1.jar
		* CoFHAPI|world (1.7.10R1.0.13) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|audio (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|gui (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|gui|container (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|gui|element (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|gui|element|listbox (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|gui|slot (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|inventory (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|render (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|render|particle (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|util (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|util|helpers (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|util|position (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|world (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* CoFHLib|world|feature (1.7.10R1.0.3) from CoFHCore-[1.7.10]3.0.3-303 (1).jar
		* ComputerCraft|API (1.74) from ComputerCraftPlusComputerCraftEdu1.74.jar
		* ComputerCraft|API|FileSystem (1.74) from EngineersToolbox-1.2.3.0-BETA.jar
		* ComputerCraft|API|Lua (1.74) from ComputerCraftPlusComputerCraftEdu1.74.jar
		* ComputerCraft|API|Media (1.74) from EngineersToolbox-1.2.3.0-BETA.jar
		* ComputerCraft|API|Peripheral (1.74) from ComputerCraftPlusComputerCraftEdu1.74.jar
		* ComputerCraft|API|Permissions (1.74) from EngineersToolbox-1.2.3.0-BETA.jar
		* ComputerCraft|API|Redstone (1.74) from ComputerCraftPlusComputerCraftEdu1.74.jar
		* ComputerCraft|API|Turtle (1.74) from ComputerCraftPlusComputerCraftEdu1.74.jar
		* computronicsAPI (1.3) from Computronics-1.7.10-1.5.7.jar
		* computronicsAPI|chat (1.3) from Computronics-1.7.10-1.5.7.jar
		* computronicsAPI|multiperipheral (1.1) from Computronics-1.7.10-1.5.7.jar
		* computronicsAPI|tape (1.0) from Computronics-1.7.10-1.5.7.jar
		* ForestryAPI|apiculture (3.5.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|arboriculture (2.3.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|circuits (2.0.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|core (3.2.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|farming (1.1.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|food (1.1.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|fuels (2.0.1) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|genetics (3.3.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|hives (4.1.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|lepidopterology (1.1) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|mail (3.0.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|recipes (3.1.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|storage (3.0.0) from forestry_1.7.10-3.6.11.2.jar
		* ForestryAPI|world (1.1.0) from forestry_1.7.10-3.6.11.2.jar
		* gendustryAPI (2.2.0) from gendustry-1.6.1.126-mc1.7.10.jar
		* IC2API (1.0) from IC2.Classic.Version.1.1.2.1.jar
		* NuclearControlAPI (v1.0.5) from IC2NuclearControl-2.3.0a-Butt.jar
		* ProjectEAPI (7) from ProjectE-1.7.10-PE1.9.3h.jar
		* RailcraftAPI|bore (1.0.0) from Railcraft_1.7.10-9.7.0.0.jar
		* RailcraftAPI|carts (1.3.1) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|core (1.4.0) from Railcraft_1.7.10-9.7.0.0.jar
		* RailcraftAPI|crafting (1.0.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|electricity (1.6.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|events (1.0.0) from Railcraft_1.7.10-9.7.0.0.jar
		* RailcraftAPI|fuel (1.0.0) from Railcraft_1.7.10-9.7.0.0.jar
		* RailcraftAPI|helpers (1.1.0) from Railcraft_1.7.10-9.7.0.0.jar
		* RailcraftAPI|items (1.0.0) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|locomotive (1.0.1) from EngineersToolbox-1.2.3.0-BETA.jar
		* RailcraftAPI|signals (1.3.4) from Railcraft_1.7.10-9.7.0.0.jar
		* RailcraftAPI|tracks (2.0.0) from Railcraft_1.7.10-9.7.0.0.jar
		* Thaumcraft|API (4.2.2.0) from Railcraft_1.7.10-9.7.0.0.jar
		* WailaAPI (1.2) from Waila-1.5.10_1.7.10.jar
	Launched Version: 1.7.10-Forge10.13.4.1492-1.7.10
	LWJGL: 2.9.1
	OpenGL: AMD Radeon R7 200 Series GL version 4.5.13399 Compatibility Profile Context 15.201.1151.0, ATI Technologies Inc.
	GL Caps: Using GL 1.3 multitexturing.
Using framebuffer objects because OpenGL 3.0 is supported and separate blending is supported.
Anisotropic filtering is supported and maximum anisotropy is 16.
Shaders are available because OpenGL 2.1 is supported.

	Is Modded: Definitely; Client brand changed to 'fml,forge'
	Type: Client (map_client.txt)
	Resource Packs: []
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	Anisotropic Filtering: Off (1)

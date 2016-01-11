==========================
Comparing Bukkit to Sponge
==========================

While the BukkitAPI is notably different to SpongAPI, there are some Events and classes which have an equivalent. This
page is intended to provide a (probably incomplete) list to help former Bukkit devs out when first trying SpongeAPI.

.. source of this table: https://gist.github.com/kashike/ecb34eb835383b05792b

.. note::
  To keep the table small, ``org.bukkit.`` and ``org.spongepowered.api.`` were removed in front of the class names.

====================================================== ===============================================================
BukkitAPI (``org.bukkit.*``)                            SpongeAPI (``org.spongepowered.api.*``)
====================================================== ===============================================================
block.banner.Pattern
block.banner.PatternType                               data.type.BannerPatternShapes
block.Banner                                           block.tileentity.Banner
block.Beacon                                           block.tileentity.carrier.Beacon
block.Biome                                            world.biome.BiomeType
block.Block                                            block.BlockState
block.BlockFace                                        util.Direction
block.BlockState                                       block.BlockSnapshot
block.BrewingStand                                     block.tileentity.carrier.BrewingStand
block.Chest                                            block.tileentity.carrier.Chest
block.CommandBlock                                     block.tileentity.CommandBlock
block.ContainerBlock                                   block.tileentity.carrier.TileEntityCarrier
block.CreatureSpawner                                  block.tileentity.MobSpawner
block.Dispenser                                        block.tileentity.carrier.Dispenser
block.DoubleChest
block.Dropper                                          block.tileentity.carrier.Dropper
block.Furnace                                          block.tileentity.carrier.Furnace
block.Hopper                                           block.tileentity.carrier.Hopper
block.Jukebox                                          block.tileentity.Jukebox
block.NoteBlock                                        block.tileentity.Note
block.PistonMoveReaction
block.Sign                                             block.tileentity.Sign
block.Skull                                            block.tileentity.Skull
command.defaults.AchievementCommand                    (none)
command.defaults.BanCommand                            (none)
command.defaults.BanIpCommand                          (none)
command.defaults.BanListCommand                        (none)
command.defaults.BukkitCommand                         (none)
command.defaults.ClearCommand                          (none)
command.defaults.DefaultGameModeCommand                (none)
command.defaults.DeopCommand                           (none)
command.defaults.DifficultyCommand                     (none)
command.defaults.EffectCommand                         (none)
command.defaults.EnchantCommand                        (none)
command.defaults.ExpCommand                            (none)
command.defaults.GameModeCommand                       (none)
command.defaults.GameRuleCommand                       (none)
command.defaults.GiveCommand                           (none)
command.defaults.HelpCommand                           (none)
command.defaults.KickCommand                           (none)
command.defaults.KillCommand                           (none)
command.defaults.ListCommand                           (none)
command.defaults.MeCommand                             (none)
command.defaults.OpCommand                             (none)
command.defaults.PardonCommand                         (none)
command.defaults.PardonIpCommand                       (none)
command.defaults.PlaySoundCommand                      (none)
command.defaults.PluginsCommand                        (none)
command.defaults.ReloadCommand                         (none)
command.defaults.SaveCommand                           (none)
command.defaults.SaveOffCommand                        (none)
command.defaults.SaveOnCommand                         (none)
command.defaults.SayCommand                            (none)
command.defaults.ScoreboardCommand                     (none)
command.defaults.SeedCommand                           (none)
command.defaults.SetIdleTimeoutCommand                 (none)
command.defaults.SetWorldSpawnCommand                  (none)
command.defaults.SpawnpointCommand                     (none)
command.defaults.SpreadPlayersCommand                  (none)
command.defaults.StopCommand                           (none)
command.defaults.TeleportCommand                       (none)
command.defaults.TellCommand                           (none)
command.defaults.TestForCommand                        (none)
command.defaults.TimeCommand                           (none)
command.defaults.TimingsCommand                        (none)
command.defaults.ToggleDownfallCommand                 (none)
command.defaults.VanillaCommand                        (none)
command.defaults.VersionCommand                        (none)
command.defaults.WeatherCommand                        (none)
command.defaults.WhitelistCommand                      (none)
command.BlockCommandSender                             command.source.CommandBlockSource
command.Command                                        command.CommandCallable
command.CommandException                               command.CommandException
command.CommandExecutor
command.CommandMap                                     (none)
command.CommandSender                                  command.CommandSource
command.ConsoleCommandSender                           command.source.ConsoleSource
command.FormattedCommandAlias                          (none)
command.MultipleCommandAlias                           (none)
command.PluginCommand                                  (none)
command.PluginCommandYamlParser                        (none)
command.PluginIdentifiableCommand                      (none)
command.ProxiedCommandSender                           command.source.ProxySource
command.RemoteConsoleCommandSender                     command.source.RconSource
command.SimpleCommandMap                               (none)
command.TabCommandExecutor                             (none)
command.TabCompleter                                   (none)
command.TabExecutor                                    (none)
configuration.file.FileConfiguration                   (none)
configuration.file.FileConfigurationOptions            (none)
configuration.file.YamlConfiguration                   (none)
configuration.file.YamlConfigurationOptions            (none)
configuration.file.YamlConstructor                     (none)
configuration.file.YamlRepresenter                     (none)
configuration.serialization.ConfigurationSerializable  (none)
configuration.serialization.ConfigurationSerialization (none)
configuration.serialization.DelegateDeserialization    (none)
configuration.serialization.SerializableAs             (none)
configuration.Configuration                            (none)
configuration.ConfigurationOptions                     (none)
configuration.ConfigurationSection                     (none)
configuration.InvalidConfigurationException            (none)
configuration.MemoryConfiguration                      (none)
configuration.MemoryConfigurationOptions               (none)
configuration.MemorySection                            (none)
conversations.BooleanPrompt
conversations.Conversable
conversations.Conversation
conversations.ConversationAbandonedEvent
conversations.ConversationAbandonedListener
conversations.ConversationCanceller
conversations.ConversationContext
conversations.ConversationFactory
conversations.ConversationPrefix
conversations.ExactMatchConversationCanceller
conversations.FixedSetPrompt
conversations.InactivityConversationCanceller
conversations.ManuallyAbandonedConversationCanceller
conversations.MessagePrompt
conversations.NullConversationPrefix
conversations.NumericPrompt
conversations.PlayerNamePrompt
conversations.PluginNameConversationPrefix
conversations.Prompt
conversations.RegexPrompt
conversations.StringPrompt
conversations.ValidatingPrompt
enchantments.Enchantment                               item.Enchantment
enchantments.EnchantmentTarget
enchantments.EnchantmentWrapper
entity.minecart.CommandMinecart                        entity.vehicle.minecart.MinecartCommandBlock
entity.minecart.ExplosiveMinecart                      entity.vehicle.minecart.MinecartTNT
entity.minecart.HopperMinecart                         entity.vehicle.minecart.MinecartHopper
entity.minecart.PoweredMinecart                        (none)
entity.minecart.RideableMinecart                       entity.vehicle.minecart.MinecartRideable
entity.minecart.SpawnerMinecart                        entity.vehicle.minecart.MinecartMobSpawner
entity.minecart.StorageMinecart                        entity.vehicle.minecart.MinecartChest
entity.Ageable                                         entity.living.Ageable
entity.Ambient                                         entity.living.Ambient
entity.Animals                                         entity.living.animal.Animal
entity.AnimalTamer                                     entity.Tamer
entity.ArmorStand                                      entity.living.ArmorStand
entity.Arrow                                           entity.projectile.Arrow
entity.Bat                                             entity.living.Bat
entity.Blaze                                           entity.living.monster.Blaze
entity.Boat                                            entity.vehicle.Boat
entity.CaveSpider                                      entity.living.monster.CaveSpider
entity.Chicken                                         entity.living.animal.Chicken
entity.ComplexEntityPart                               entity.living.complex.ComplexLivingPart
entity.ComplexLivingEntity                             entity.living.complex.ComplexLiving
entity.Cow                                             entity.living.animal.Cow
entity.Creature                                        entity.living.Creature
entity.CreatureType                                    (none)
entity.Creeper                                         entity.living.monster.Creeper
entity.Damageable                                      (none)
entity.Egg                                             entity.projectile.Egg
entity.EnderCrystal                                    entity.EnderCrystal
entity.EnderDragon                                     entity.living.complex.EnderDragon
entity.EnderDragonPart                                 entity.living.complex.EnderDragonPart
entity.Enderman                                        entity.living.monster.Enderman
entity.Endermite                                       entity.living.monster.Endermite
entity.EnderPearl                                      entity.projectile.EnderPearl
entity.EnderSignal                                     entity.projectile.EyeOfEnder
entity.Entity                                          entity.Entity
entity.EntityType                                      entity.EntityType
entity.ExperienceOrb                                   entity.ExperienceOrb
entity.Explosive                                       entity.explosive.Explosive
entity.FallingBlock                                    entity.FallingBlock
entity.FallingSand                                     (none)
entity.Fireball                                        entity.projectile.explosive.fireball.Fireball
entity.Firework                                        entity.projectile.Firework
entity.Fish                                            (none)
entity.FishHook                                        entity.projectile.FishHook
entity.Flying                                          entity.living.Aerial
entity.Ghast                                           entity.living.monster.Ghast
entity.Giant                                           entity.living.monster.Giant
entity.Golem                                           entity.living.golem.Golem
entity.Guardian                                        entity.living.monster.Guardian
entity.Hanging                                         entity.hanging.Hanging
entity.Horse                                           entity.living.animal.Horse
entity.HumanEntity                                     entity.living.Humanoid
entity.IronGolem                                       entity.living.golem.IronGolem
entity.Item                                            entity.Item
entity.ItemFrame                                       entity.hanging.ItemFrame
entity.LargeFireball                                   entity.projectile.explosive.fireball.LargeFireball
entity.LeashHitch                                      entity.hanging.LeashHitch
entity.LightningStrike                                 entity.weather.Lightning
entity.LivingEntity                                    entity.living.Living
entity.MagmaCube                                       entity.living.monster.MagmaCube
entity.Minecart                                        entity.vehicle.minecart.Minecart
entity.Monster                                         entity.living.monster.Monster
entity.MushroomCow                                     entity.living.animal.Mooshroom
entity.NPC                                             (none)
entity.Ocelot                                          entity.living.animal.Ocelot
entity.Painting                                        entity.hanging.Painting
entity.Pig                                             entity.living.animal.Pig
entity.PigZombie                                       entity.living.monster.ZombiePigman
entity.Player                                          entity.living.player.Player
entity.PoweredMinecart                                 (none)
entity.Projectile                                      entity.projectile.Projectile
entity.Rabbit                                          entity.living.animal.Rabbit
entity.Sheep                                           entity.living.animal.Sheep
entity.Silverfish                                      entity.living.monster.Silverfish
entity.Skeleton                                        entity.living.monster.Skeleton
entity.Slime                                           entity.living.monster.Slime
entity.SmallFireball                                   entity.projectile.explosive.fireball.SmallFireball
entity.Snowball                                        entity.projectile.Snowball
entity.Snowman                                         entity.living.golem.SnowGolem
entity.Spider                                          entity.living.monster.Spider
entity.Squid                                           entity.living.Squid
entity.StorageMinecart                                 entity.vehicle.minecart.MinecartChest
entity.Tameable
entity.ThrownExpBottle                                 entity.projectile.ThrownExpBottle
entity.ThrownPotion                                    entity.projectile.ThrownPotion
entity.TNTPrimed                                       entity.explosive.PrimedTNT
entity.Vehicle
entity.Villager                                        entity.living.Villager
entity.WaterMob                                        entity.living.Aquatic
entity.Weather                                         entity.weather.WeatherEffect
entity.Witch                                           entity.living.monster.Witch
entity.Wither                                          entity.living.monster.Wither
entity.WitherSkull                                     entity.projectile.explosive.WitherSkull
entity.Wolf                                            entity.living.animal.Wolf
entity.Zombie                                          entity.living.monster.Zombie
event.block.Action                                     (none)
event.block.BlockBreakEvent                            event.block.ChangeBlockEvent.Break
event.block.BlockBurnEvent
event.block.BlockCanBuildEvent
event.block.BlockDamageEvent
event.block.BlockDispenseEvent
event.block.BlockEvent                                 event.block.TargetBlockEvent
event.block.BlockExpEvent
event.block.BlockExplodeEvent
event.block.BlockFadeEvent
event.block.BlockFormEvent
event.block.BlockFromToEvent
event.block.BlockGrowEvent                             event.block.ChangeBlockEvent.Grow
event.block.BlockIgniteEvent
event.block.BlockMultiPlaceEvent                       event.block.ChangeBlockEvent.Place
event.block.BlockPhysicsEvent
event.block.BlockPistonEvent
event.block.BlockPistonExtendEvent
event.block.BlockPistonRetractEvent
event.block.BlockPlaceEvent                            event.block.ChangeBlockEvent.Place
event.block.BlockRedstoneEvent
event.block.BlockSpreadEvent
event.block.EntityBlockFormEvent
event.block.LeavesDecayEvent
event.block.NotePlayEvent
event.block.SignChangeEvent                            event.block.tileentity.ChangeSignEvent
event.enchantment.EnchantItemEvent
event.enchantment.PrepareItemEnchantEvent
event.entity.CreatureSpawnEvent
event.entity.CreeperPowerEvent
event.entity.EntityBreakDoorEvent
event.entity.EntityChangeBlockEvent
event.entity.EntityCombustByBlockEvent
event.entity.EntityCombustByEntityEvent
event.entity.EntityCombustEvent
event.entity.EntityCreatePortalEvent
event.entity.EntityDamageByBlockEvent
event.entity.EntityDamageByEntityEvent
event.entity.EntityDamageEvent                         event.entity.DamageEntityEvent
event.entity.EntityDeathEvent                          event.entity.DestructEntityEvent.Death
event.entity.EntityEvent                               event.entity.TargetEntityEvent
event.entity.EntityExplodeEvent
event.entity.EntityInteractEvent
event.entity.EntityPortalEnterEvent
event.entity.EntityPortalEvent
event.entity.EntityPortalExitEvent
event.entity.EntityRegainHealthEvent
event.entity.EntityShootBowEvent
event.entity.EntityTameEvent
event.entity.EntityTargetEvent
event.entity.EntityTargetLivingEntityEvent
event.entity.EntityTeleportEvent
event.entity.EntityUnleashEvent
event.entity.ExpBottleEvent
event.entity.ExplosionPrimeEvent
event.entity.FireworkExplodeEvent
event.entity.FoodLevelChangeEvent
event.entity.HorseJumpEvent
event.entity.ItemDespawnEvent
event.entity.ItemMergeEvent
event.entity.ItemSpawnEvent
event.entity.PigZapEvent
event.entity.PlayerDeathEvent
event.entity.PlayerLeashEntityEvent
event.entity.PotionSplashEvent
event.entity.ProjectileHitEvent
event.entity.ProjectileLaunchEvent
event.entity.SheepDyeWoolEvent
event.entity.SheepRegrowWoolEvent
event.entity.SlimeSplitEvent
event.hanging.HangingBreakByEntityEvent
event.hanging.HangingBreakEvent
event.hanging.HangingEvent
event.hanging.HangingPlaceEvent
event.inventory.BrewEvent
event.inventory.ClickType
event.inventory.CraftItemEvent
event.inventory.DragType
event.inventory.FurnaceBurnEvent
event.inventory.FurnaceExtractEvent
event.inventory.FurnaceSmeltEvent
event.inventory.InventoryAction
event.inventory.InventoryClickEvent
event.inventory.InventoryCloseEvent
event.inventory.InventoryCreativeEvent
event.inventory.InventoryDragEvent
event.inventory.InventoryEvent
event.inventory.InventoryInteractEvent
event.inventory.InventoryMoveItemEvent
event.inventory.InventoryOpenEvent
event.inventory.InventoryPickupItemEvent
event.inventory.InventoryType
event.inventory.PrepareItemCraftEvent
event.painting.PaintingBreakByEntityEvent
event.painting.PaintingBreakEvent
event.painting.PaintingEvent
event.painting.PaintingPlaceEvent
event.player.AsyncPlayerChatEvent
event.player.AsyncPlayerPreLoginEvent
event.player.PlayerAchievementAwardedEvent             event.achievement.GrantAchievementEvent.TargetPlayer
event.player.PlayerAnimationEvent
event.player.PlayerAnimationType
event.player.PlayerArmorStandManipulateEvent
event.player.PlayerBedEnterEvent
event.player.PlayerBedLeaveEvent
event.player.PlayerBucketEmptyEvent
event.player.PlayerBucketEvent
event.player.PlayerBucketFillEvent
event.player.PlayerChangedWorldEvent
event.player.PlayerChannelEvent
event.player.PlayerChatEvent
event.player.PlayerChatTabCompleteEvent
event.player.PlayerCommandPreprocessEvent
event.player.PlayerDropItemEvent
event.player.PlayerEditBookEvent
event.player.PlayerEggThrowEvent
event.player.PlayerEvent                               event.entity.living.humanoid.player.TargetPlayerEvent
event.player.PlayerExpChangeEvent
event.player.PlayerFishEvent
event.player.PlayerGameModeChangeEvent                 event.entity.living.humanoid.ChangeGameModeEvent.TargetPlayer
event.player.PlayerInteractAtEntityEvent
event.player.PlayerInteractEntityEvent
event.player.PlayerInteractEvent
event.player.PlayerInventoryEvent
event.player.PlayerItemBreakEvent
event.player.PlayerItemConsumeEvent
event.player.PlayerItemHeldEvent
event.player.PlayerJoinEvent
event.player.PlayerKickEvent                           event.entity.living.humanoid.player.KickPlayerEvent
event.player.PlayerLevelChangeEvent
event.player.PlayerLoginEvent
event.player.PlayerMoveEvent                           event.entity.DisplaceEntityEvent.Move.TargetPlayer
event.player.PlayerPickupItemEvent
event.player.PlayerPortalEvent
event.player.PlayerPreLoginEvent
event.player.PlayerQuitEvent
event.player.PlayerRegisterChannelEvent
event.player.PlayerResourcePackStatusEvent             event.entity.living.humanoid.player.ResourcePackStatusEvent
event.player.PlayerRespawnEvent                        event.entity.living.humanoid.player.RespawnPlayerEvent
event.player.PlayerShearEntityEvent
event.player.PlayerStatisticIncrementEvent             event.statistic.ChangeStatisticEvent.TargetPlayer
event.player.PlayerTeleportEvent                       event.entity.DisplaceEntityEvent.Teleport.TargetPlayer
event.player.PlayerToggleFlightEvent
event.player.PlayerToggleSneakEvent
event.player.PlayerToggleSprintEvent
event.player.PlayerUnleashEntityEvent
event.player.PlayerUnregisterChannelEvent
event.player.PlayerVelocityEvent
event.server.MapInitializeEvent
event.server.PluginDisableEvent
event.server.PluginEnableEvent
event.server.PluginEvent
event.server.RemoteServerCommandEvent
event.server.ServerCommandEvent
event.server.ServerEvent
event.server.ServerListPingEvent                       event.server.ClientPingServerEvent
event.server.ServiceEvent
event.server.ServiceRegisterEvent
event.server.ServiceUnregisterEvent
event.vehicle.VehicleBlockCollisionEvent
event.vehicle.VehicleCollisionEvent
event.vehicle.VehicleCreateEvent
event.vehicle.VehicleDamageEvent
event.vehicle.VehicleDestroyEvent
event.vehicle.VehicleEnterEvent
event.vehicle.VehicleEntityCollisionEvent
event.vehicle.VehicleEvent
event.vehicle.VehicleExitEvent
event.vehicle.VehicleMoveEvent
event.vehicle.VehicleUpdateEvent
event.weather.LightningStrikeEvent
event.weather.ThunderChangeEvent
event.weather.WeatherChangeEvent                       event.world.ChangeWorldWeatherEvent
event.weather.WeatherEvent
event.world.ChunkEvent                                 event.world.chunk.TargetChunkEvent
event.world.ChunkLoadEvent                             event.world.chunk.LoadChunkEvent
event.world.ChunkPopulateEvent                         event.world.chunk.PopulateChunkEvent
event.world.ChunkUnloadEvent                           event.world.chunk.UnloadChunkEvent
event.world.PortalCreateEvent
event.world.SpawnChangeEvent
event.world.StructureGrowEvent
event.world.WorldEvent                                 event.world.TargetWorldEvent
event.world.WorldInitEvent                             event.world.ConstructWorldEvent
event.world.WorldLoadEvent                             event.world.LoadWorldEvent
event.world.WorldSaveEvent                             event.world.SaveWorldEvent
event.world.WorldUnloadEvent                           event.world.UnloadWorldEvent
event.Cancellable                                      event.Cancellable
event.Event                                            event.Event
event.EventException
event.EventHandler                                     event.Listener
event.EventPriority                                    event.Order
event.HandlerList
event.Listener
generator.BlockPopulator
generator.ChunkGenerator
help.GenericCommandHelpTopic
help.HelpMap
help.HelpTopic
help.HelpTopicComparator
help.HelpTopicFactory
help.IndexHelpTopic
inventory.meta.BannerMeta
inventory.meta.BlockStateMeta
inventory.meta.BookMeta
inventory.meta.EnchantmentStorageMeta
inventory.meta.FireworkEffectMeta
inventory.meta.FireworkMeta
inventory.meta.ItemMeta
inventory.meta.LeatherArmorMeta
inventory.meta.MapMeta
inventory.meta.PotionMeta
inventory.meta.Repairable
inventory.meta.SkullMeta
inventory.AnvilInventory
inventory.BeaconInventory
inventory.BrewerInventory
inventory.CraftingInventory
inventory.DoubleChestInventory
inventory.EnchantingInventory
inventory.EntityEquipment
inventory.EquipmentSlot
inventory.FurnaceInventory
inventory.FurnaceRecipe
inventory.HorseInventory
inventory.Inventory
inventory.InventoryHolder
inventory.InventoryView
inventory.ItemFactory
inventory.ItemFlag
inventory.ItemStack
inventory.MerchantInventory
inventory.PlayerInventory
inventory.Recipe
inventory.ShapedRecipe
inventory.ShapelessRecipe
map.MapCanvas
map.MapCursor
map.MapCursorCollection
map.MapFont
map.MapPalette
map.MapRenderer
map.MapView
map.MinecraftFont
material.Attachable
material.Banner
material.Bed
material.Button
material.Cake
material.Cauldron
material.Chest
material.Coal
material.CocoaPlant
material.Colorable
material.Command
material.Crops
material.DetectorRail
material.Diode
material.Directional
material.DirectionalContainer
material.Dispenser
material.Door
material.Dye
material.EnderChest
material.ExtendedRails
material.FlowerPot
material.Furnace
material.FurnaceAndDispenser
material.Gate
material.Ladder
material.Leaves
material.Lever
material.LongGrass
material.MaterialData
material.MonsterEggs
material.Mushroom
material.NetherWarts
material.Openable
material.PistonBaseMaterial
material.PistonExtensionMaterial
material.PoweredRail
material.PressurePlate
material.PressureSensor
material.Pumpkin
material.Rails
material.Redstone
material.RedstoneTorch
material.RedstoneWire
material.Sandstone
material.Sign
material.SimpleAttachableMaterialData
material.Skull
material.SmoothBrick
material.SpawnEgg
material.Stairs
material.Step
material.TexturedMaterial
material.Torch
material.TrapDoor
material.Tree
material.Tripwire
material.TripwireHook
material.Vine
material.WoodenStep
material.Wool
metadata.FixedMetadataValue
metadata.LazyMetadataValue
metadata.Metadatable
metadata.MetadataConversionException
metadata.MetadataEvaluationException
metadata.MetadataStore
metadata.MetadataStoreBase
metadata.MetadataValue
metadata.MetadataValueAdapter
permissions.Permissible                                service.permission.Subject
permissions.PermissibleBase
permissions.Permission
permissions.PermissionAttachment
permissions.PermissionAttachmentInfo
permissions.PermissionDefault
permissions.PermissionRemovedExecutor
permissions.ServerOperator
plugin.java.JavaPlugin
plugin.java.PluginLoader
plugin.java.PluginClassLoader
plugin.messaging.ChannelNameTooLongException
plugin.messaging.ChannelNotRegisteredException
plugin.messaging.MessageTooLargeException
plugin.messaging.Messenger
plugin.messaging.PluginChannelDirection
plugin.messaging.PluginMessageListener
plugin.messaging.PluginMessageListenerRegistration
plugin.messaging.PluginMessageRecipient
plugin.messaging.ReservedChannelException
plugin.messaging.StandardMessenger
plugin.AuthorNagException
plugin.EventExecutor
plugin.IllegalPluginAccessException
plugin.InvalidDescriptionException
plugin.InvalidPluginException
plugin.Plugin
plugin.PluginAwareness
plugin.PluginBase
plugin.PluginDescriptionFile
plugin.PluginLoader
plugin.PluginLoadOrder
plugin.PluginLogger
plugin.PluginManager                                   plugin.PluginManager
plugin.RegisteredListener
plugin.RegisteredServiceProvider
plugin.ServicePriority
plugin.ServicesManager                                 service.ServiceManager
plugin.SimplePluginManager
plugin.SimpleServicesManager                           service.SimpleServiceManager
plugin.TimedRegisteredListener
plugin.UnknownDependencyException
potion.Potion
potion.PotionBrewer
potion.PotionEffect                                    effect.potion.PotionEffect
potion.PotionEffectType                                effect.potion.PotionEffectType
potion.PotionEffectTypeWrapper
potion.PotionType
projectiles.BlockProjectileSource
projectiles.ProjectileSource
scheduler.BukkitRunnable
scheduler.BukkitScheduler
scheduler.BukkitTask                                   scheduler.Task
scheduler.BukkitWorker
scoreboard.Criterias                                   scoreboard.critieria.Criterion
scoreboard.DisplaySlot                                 scoreboard.displayslot.DisplaySlot
scoreboard.NameTagVisibility                           scoreboard.Visibility
scoreboard.Objective                                   scoreboard.objective.Objective
scoreboard.Score                                       scoreboard.Score
scoreboard.Scoreboard                                  scoreboard.Scoreboard
scoreboard.ScoreboardManager
scoreboard.Team                                        scoreboard.Team
util.io.BukkitObjectInputStream
util.io.BukkitObjectOutputStream
util.io.Wrapper
util.noise.NoiseGenerator
util.noise.OctaveGenerator
util.noise.PerlinNoiseGenerator
util.noise.PerlinOctaveGenerator
util.noise.SimplexNoiseGenerator
util.noise.SimplexOctaveGenerator
util.permissions.BroadcastPermissions
util.permissions.CommandPermissions
util.permissions.DefaultPermissions
util.BlockIterator
util.BlockVector
util.CachedServerIcon
util.ChatPaginator
util.EulerAngle
util.FileUtil
util.Java15Compat
util.NumberConversions
util.StringUtil
util.Vector
Achievement                                            statistic.achievement.Achievement
Art                                                    data.type.Art
BanEntry                                               util.ban.Ban
BanList
BlockChangeDelegate
Bukkit                                                 Sponge
ChatColor
Chunk                                                  world.Chunk
ChunkSnapshot
CoalType                                               data.type.CoalType
Color                                                  util.Color
CropState
Difficulty                                             world.difficulty.Difficulty
DyeColor                                               data.type.DyeColor
Effect
EntityEffect
FireworkEffect
GameMode                                               entity.living.player.gamemode.GameMode
GrassSpecies
Instrument                                             data.type.InstrumentType
Location
Material
NetherWartsState
Note
OfflinePlayer                                          entity.living.player.User
PortalType
Rotation
SandstoneType                                          data.type.SandstoneType
Server                                                 Server
SkullType                                              data.type.SkullType
Sound                                                  effect.sound.SoundType
Statistic                                              statistic.Statistic
TravelAgent
TreeSpecies                                            data.type.TreeType
TreeType
UnsafeValues                                           (none)
Utility                                                (none)
Warning                                                (none)
WeatherType                                            world.weather.Weather
World                                                  world.World
WorldBorder                                            world.WorldBorder
WorldCreator                                           world.WorldCreationSettings.Builder
WorldType                                              world.GeneratorType
====================================================== ===============================================================

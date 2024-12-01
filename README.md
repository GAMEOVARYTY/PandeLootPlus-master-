name: PandeLoot
main: net.seyarada.pandeloot.PandeLoot
version: dev
api-version: 1.17
softdepend: [MythicMobs, MMOItems]
commands:
  pandeloot:
    description: Base command for PandeLoot
    usage: /pandeloot
    permission: pandeloot.use
    aliases:
      - ploot
      MyExampleTable:
  Rewards:
    - diamond{explode=true;glow=true}
    - diamond{explode=true;glow=true;color=RED}
    - diamond{explode=true;glow=true;color=YELLOW}
    # Test comment here
SomeFlag:
  Message: 'hello'
# Another test comment here
# Only use this file for making *vanilla* mobs drop PandeLoot rewards
# or mob plugins that haven't been added to the compatibility list yet
# For MythicMobs and similar, check the compatibility page at the wiki
ExampleMob:
  Type: Wither_Skeleton
  Display: 'Great Skeleton Boss'
  World: some_world
  Rewards:
  - coal
  Options:
    ScoreHologram: false
    onBlockBreak:
  Enabled: false
  Flags: '{glow=true;color=BLUE}'
Settings:
  Debug: false
  IgnoreCitizensDamage: true
Announcements:
  ScoreHologram:
    - '&8&m========================'
    - '%mob.name% &7- &a%mob.hp%HP'
    - '&e#1 &7|&b &f%1.name% &7|&b %1.dmg%%'
    - '&6#2 &7|&b &f%2.name% &7|&b %2.dmg%%'
    - '&3#3 &7|&b &f%3.name% &7|&b %3.dmg%%'
    - ''
    - 'Your rank: &a#%player.rank% | %player.damage%'
    - '&8&m========================'
  ScoreMessage:
    - '&8&m========================================'
    - '%mob.name% &7- &a%mob.hp%HP'
    - '&e#1 &7|&b &f%1.name% &7|&b %1.dmg%%'
    - '&6#2 &7|&b &f%2.name% &7|&b %2.dmg%%'
    - '&3#3 &7|&b &f%3.name% &7|&b %3.dmg%%'
    - ''
    - 'Your rank: &a#%player.rank%'
    - '&8&m========================================'
DefaultFlag:
  Glow: true
  Explode: true
  Visibility: player
  VoidProtection: 50
onBlockBreak:
  Enabled: false
  Flags: '{glow=true;color=AQUA;visibility=player}'
onBlockBreakMMO:
  Enabled: false
  Flags: '{glow=true;color=AQUA;visibility=player}'
onPlayerItemDrop:
  Enabled: false
  Flags: '{glow=true;color=GREEN;visibility=player}'

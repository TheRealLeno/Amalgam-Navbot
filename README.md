# Amalgam-Navbot
Original github.com/rei-2/Amalgam

Features

NavBot and Nav Engine
The NavBot module is more than basic roaming. It reads TF2 .nav meshes, finds paths, follows waypoint “crumbs,” checks visibility/traversability, and tracks stuck or failed routes. It also has path-worker support, nav-area/path visualization, hazard costs, and blacklist/repath handling.

Its jobs include:

Objectives: seek or capture control points, payload goals, CTF flags, Pass Time goals, and Doomsday goals.
Engineer: choose building spots, build sentries/dispensers, maintain them, and select defensive focus points.
Survival and supplies: escape spawn or danger, react to projectiles, seek health/ammo and dispensers, reload safely, and fight nearby enemies with melee.
Team and map behavior: roam/patrol or defend, stay near/follow a selected player, group with others, and target sentries. There is also an MvM Sniper behavior.
Options: job preferences (health, ammo, reload, objectives, danger, Engineer, etc.), Yolo/Balanced/Cautious personalities, smart jumping, double-tap recharge options, danger blacklists, melee range, and a danger overlay.
The separate Nav Engine settings expose path/area/blacklist drawing, colors, stuck detection/blacklist timing, and visibility-check caching.

FollowBot follows configured teammates or enemies, supports target priorities and friend/party preferences, can use navmesh paths, has look-at-path modes, configurable follow/abandon distances, and optional path drawing.

AutoJoin and class selection
AutoJoin can:

Force a selected class: Off, Scout, Soldier, Pyro, Demoman, Heavy, Engineer, Medic, Sniper, or Spy.
Choose a random class, exclude selected classes, and change class on a configurable interval (default range: 3–5 minutes).
Request a team automatically first if the player is not on RED/BLU, then issue the class request.
Display a runtime status message describing what it is waiting for or has requested.
The source itself has a note that AutoJoin may not work with custom HUDs.

Queueing, requeueing, votes, and items
AutoQueue supports automatic Casual, Competitive, Mann Up, and Boot Camp queueing, Casual joining, region/queue options, and profile dumping. Requeue options can use player-count conditions, ignore friends/party/tagged players, cancel while a map is loading, or avoid abandoning the current match.
AutoVote can respond to votes based on player priorities, friends, party members, ignored players, and configured defend/assist/kick behavior; it also has optional delays and map-vote settings.
AutoItem automates configured weapon/item loadouts, hats, noisemakers, item renting/crafting, and some achievement-item handling.

Combat and movement
Aimbot has global targeting plus Hitscan, Projectile, and Melee modules, alongside AutoAirblast, AutoDetonate, AutoHeal, and AutoRocketJump.
Separate NoSpread, Backtrack, Resolver, and CritHack modules.
PacketManip includes AntiAim and FakeLag; Ticks and Simulation cover tick-related behavior and movement/projectile simulation.
Misc contains movement helpers and assorted automation such as anti-AFK, auto-retry, auto-disguise, chat/voice automation, and related game options.

Visuals and interface
Visuals includes ESP, Chams, Glow, Materials, Offscreen Arrows, Fake Angle, Groups, Player Conditions, Spectator List, and Camera Window. World handles world-related visuals/settings.

The ImGui interface includes the menu, dashboard, binds, configs, notifications, output/logging, indicators, and visual settings. Other support modules include Commands, Configs, Binds, CheatDetection, and AntiCheatCompatibility.

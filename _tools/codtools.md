---
layout: post
title: CODTools
img: assets/tools/codtools.png
description: "Exports xmodel, xanim export and bin files directly from Maya (2013+)"
order: 2
date: 2019-01-04
---

# CODTools (Autodesk Maya Exporter)
Exports `xmodel, xanim` export and bin files directly from Maya (2013+).

## Installation:

Download the latest [CODTools](https://mega.nz/#!REA3GaKJ!zGPZkugi8VDo7Ce0XMpQ1L7eq8evJrG5dWMgfdzyTdM) for your Maya **version** and **arch**, and save it in the following directory depending on your OS and Maya version:
- 32bit Windows: C:\Program Files(x86)\AutoDesk\Maya-ver\bin\plug-ins\
- 64bit Windows: C:\Program Files\AutoDesk\Maya-ver\bin\plug-ins\

Next, you must open the plugin manager using `Window->Settings/Preferences->Plugin Manager` once there find `CODTools.nll.dll` and check off the following:
- Loaded (Loads the plugin)
- Auto load (Loads the plugin every launch)

## Updating:

Replace the files in the correct directory from the installation section with the new ones (While Maya is closed). Then simply relaunch Maya.

## Usage:

_Models:_
- To export a model quickly, either select what you would like to export, or, select nothing and it will export everything. Use the `CODTools->Export XModel` command to save the file.
- To export a !!Siege Model!! use `File->Export All` then check off the siege model export setting before saving.
- To export a model with !!Cosmetic Bones!!, use `File->Export All` then enter in the tag name of the cosmetic root bone.

_Animations:_

- To export an animation quickly, set the scene time, then select the bones to export, or select nothing to export all. Use the `CODTools->Export XAnim` command to save the file.
- To export a !!Siege Anim!! use `File->Export All` then select the `CoD SIEGE_ANIM_SOURCE` type before saving.
- By default, SEAnim notetracks will be added to the anim, you can turn this off via `File->Export All` configuration.

## Changelog:
_6/15/2018:_
- Fixed XAnim notetracks with weird strings

_Previous Versions:_
- Default XAnim version lower for backwards compatibility...
- Fixed issue with skin binds in other Maya versions.
- Automatic quad to tris conversion
- Fixed duplicate mesh writing
- Fixed XAnim last frame
- Fixed material mapping on some models
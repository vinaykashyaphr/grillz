# Grillz POC: User Guide

This app lets you take a 3D scan of a dental arch, mark out the area you
want to cover, and generate a gold shell — optionally set with diamonds 
that you can preview and export as an STL file.

## Getting Started

Open the app link you were given. It loads with a sample scan so you can
try it out right away, or you can load your own scan using the panel on
the left.

**Camera controls**
- **Drag**: rotate the view
- **Right-drag**: pan
- **Scroll wheel**: zoom

## Step 1: Load a Scan

Under **1 · Scan**, click the file field and choose an `.stl` file of the
arch you want to work with.

## Step 2" Mark the Region

Under **2 · Region and stone areas**, choose one of three tools:

- **Outline**:  click points along the boundary of the area you want
  covered; the line snaps to the scan surface as you go. Press **Enter**
  to close the loop, the enclosed area fills in automatically. If it
  fills the wrong side, hold **Shift** and press **Enter** instead, then
  click inside the area you actually want.
- **Quick**: click individual teeth/faces to add them directly.
  **Shift+click** grows the selection to nearby connected area;
  **Alt+click** removes it. The **Angle limit** slider controls how far
  the "connected" selection spreads.
- **Stone area**: same as Outline, but marks a region where diamonds
  should be placed later (Step 3), separate from the shell region.

Other controls in this section:
- **Close and fill**: same as pressing Enter
- **Clear all**: resets the current selection and stone areas

## Step 3:  Add Stones (Optional)

Under **3 · Stones**:
- Switch **Decoration** to **Diamonds** to place stones inside any stone
  areas you marked in Step 2.
- Choose a **pattern**: Straight or Honeycomb.
- Adjust **stone size**, **gap between stones**, **stone margin**, and
  **prong size** with the sliders to fine-tune the layout.

## Step 4 — Generate the Shell

Under **4 · Shell**, adjust the **Thickness** slider, then click
**Generate shell**. This builds the gold shell over your marked region.

## Viewing and Exporting

Under **View and export**:
- **Scan / Combined / Jewellery**: switch between the raw scan, the
  scan with the shell overlaid, or the shell (and stones) on their own.
- **Focus**: center the camera on the shell, or on your current
  selection if no shell exists yet.
- **Download STL**: exports the finished shell (with stones, if any) as
  an `.stl` file you can download and open elsewhere.

## Undo / Redo

Use the **Undo** and **Redo** buttons in the top panel (or **Ctrl+Z** /
**Ctrl+Y**) to step back and forward through your region and stone-area
changes.

## Tips

- You can hide the side panel at any time using the **Hide** button in
  the top-left corner to get an unobstructed view.
- If something looks off (a shell fails to generate, or a scan won't
  load), open the **Debug log** at the bottom of the panel for details,
  and use **Copy log** if you need to share it.

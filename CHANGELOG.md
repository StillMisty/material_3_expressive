## 1.1.7

### Changed

* Raise `material_ui` to `^1.7.0`.

## 1.1.6

### Changed

* Raise `material_ui` to `^1.6.0`.
* **Carousel:** `M3ECarouselScrim.gradient`, with a default bottom scrim fade.
* **Sliders:** larger, full-strength tick marks that match the end stops.

### Fixed

* **Bottom sheets:** no bounce back up when content or system bars resize
  while closing ([#28](https://github.com/paadevelopments/material_3_expressive/pull/28),
  thanks @StillMisty).

## 1.1.5

### Changed

* **Search:** spec pill bar, contained or divided view and `M3ESliverSearchBar`.
* **Text fields:** spec filled and outlined fields with new slots, counter,
  clear and password buttons; `maxLines` is now `int?`.
* **Dialogs:** spec basic and full-screen dialogs, spring motion, focus trap,
  `M3EDialogController` and `M3EDialog.showAdaptive`.
* **Bottom sheets:** spec sheets with preset heights, `.standard`,
  `M3EBottomSheetController` and `.showAdaptive`; new `handleVerticalPadding`
  and `dismissVelocity` defaults.
* **Side sheets:** spec modal, standard and detached sheets,
  `M3ESideSheetLayout` and `M3ESideSheetController`.
* **Buttons:** `M3EButtonDecorationScope` and live state layers.
* **Lists:** expandable row fill, sublist corners and single Tab stop with
  arrow keys.
* **Breaking — side sheets:** `M3ESideSheetTheme` was rebuilt.
  `cornerRadius` → `modalCornerRadius`; `headerPadding` → `horizontalPadding`,
  `startPaddingWithIcon`, `headerVerticalPadding`, `topElementsGap`;
  `actionsPadding` → `actionsTopPadding`, `actionsBottomPadding`,
  `horizontalPadding`; `closeButtonPadding` and `iconSize` removed;
  `containerColor(scheme)` now takes the variant; `titleStyle()` →
  `headlineStyle()`.
* **Breaking — text fields:** `M3ETextFieldTheme` was rebuilt. `minHeight` →
  `containerHeight`; `iconGap` → `iconTextGap` / `iconEdgePadding`;
  `supportingTextPadding` → `supportingTopPadding` /
  `supportingHorizontalPadding`; `horizontalPadding` is now a `double`;
  colors move to `colors: M3ETextFieldColorTheme(...)` / `resolveColors()`.
  Removed `contentHeight`, `contentVerticalPadding`, `labelRestingOffset`,
  `labelFloatingTopPadding`, `labelRestingTopPadding`, `labelBottomPadding`,
  `labelSlotHeight()`, `accentColor()`, `backgroundDecoration()`,
  `borderDecoration()` and `decoration()`.

### Fixed

* **Text fields (web):** typing works after refocusing a reconfigured field.
* **Text fields, search:** touch selection shows the selection handles.
* **Lists:** `M3EList.sliver` no longer throws in a `CustomScrollView`.

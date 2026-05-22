# Alarm Time Picker

## Use When

Use for alarm creation, time selection, scheduling, countdowns, reminders, or
routine setup.

## Anatomy

- large time or picker wheels
- selected hour and minute
- repeat/sound/snooze options
- confirmation action
- cancel action
- ambient time grid or timeline

## Layout Rules

- Time is the object.
- Selected values should sit near optical center.
- Secondary options sit below or around the picker, not above it.
- Confirmation belongs in the bottom action zone.

## State Rules

- default: current time selection visible
- pressed: option and confirm controls respond
- scrolling: picker values move with depth or fade
- disabled: invalid option is muted
- loading: confirm action shows progress
- error: invalid schedule keeps selected values visible
- success: show next alarm time clearly

## Motion Rules

- Wheel or timeline movement can be kinetic.
- Snap to selected value.
- Avoid excessive easing that makes time feel imprecise.

## Accessibility

- Provide direct input or step controls when possible.
- Announce selected hour and minute.
- Do not make repeat/sound/snooze dependent on tiny icons only.

## Anti-Slop Checks

- Fails if time is smaller than labels.
- Fails if confirmation is ambiguous.
- Fails if selected value is only shown by color.

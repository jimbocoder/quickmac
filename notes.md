Copyq

Obsidian
Touchpad:
Tap to click
3-finger drag
Possibly: defaults -currentHost write NSGlobalDomain com.apple.trackpad.threeFingerSwipeGesture -int 1
Kb repeat rate
Clock HH:MM:SS
Battery pct in bar
Install all the stuff in onboarding doc
Quick lock hotcorner
Karabiner (elements / seil?) (brew karabiner-elements)




## karabiner
{
    "description": "Change caps_lock to left_control. (or escape if pressed alone)",
    "manipulators": [
        {
            "from": {
                "key_code": "caps_lock",
                "modifiers": {
                    "optional": [
                        "any"
                    ]
                }
            },
            "to": [
                {
                    "key_code": "left_control"
                }
            ],
            "to_if_alone": [
                {
                    "key_code": "escape"
                }
            ],
            "type": "basic"
        }
    ]
}





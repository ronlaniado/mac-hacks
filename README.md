# Mac Hacks

## Useful terminal commands to make macOS suck less



Download apps from everywhere (not just identified, trusted developers)

`sudo spctl --master-disable` 



Enroll in Developer Beta

`sudo /System/Library/PrivateFrameworks/Seeding.framework/Versions/A/Resources/seedutil enroll DeveloperSeed`



Remove the Dock autohide delay

`defaults write com.apple.dock autohide-delay -float 0; killall Dock`



Instead of typing in your password for `sudo`, you can use TouchID instead

`sudo sed -i '' -e "1s/^//p; 1s/^.*/auth    sufficient   pam_tid.so/" /etc/pam.d/sudo`




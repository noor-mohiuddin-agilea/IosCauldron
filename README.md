### Setup Instructions

1. Update ERN platform to 0.35.0

  + `ern platform use 0.35.0`
  
2. Setup the cauldron

  + `ern cauldron repo add IosCauldron git@github.com:noor-mohiuddin-agilea/IosCauldron.git`
  
3. Generate ERN container locally
  
  + `rm -rf ~/.ern/containergen/out/ios;`
  + `ern cauldron repo use IosCauldron && ern create-container --platform ios --outDir ~/.ern/containergen/out/ios`

4. Run the cauldron

  + `ern start`

5. Clone Native Ios repo

  + `git clone git@github.com:noor-mohiuddin-agilea/ERNativeIos.git`
  + Open ERNativeIos project in XCode
  + Build and run the native ios application on an iOS simulator or device
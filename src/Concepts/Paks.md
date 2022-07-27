# Pak files
- Pak files are essentially archive files that store most of the resources that the game in question requires to run (think of them as custom .zip files)
- The game's main pak will always be contained in the `Content/Paks` directory
- Pak files will sometimes be encrypted via AES keys, however these can be easilyfound  with [AESKeyFinder](https://zenhax.com/viewtopic.php?t=9407&start=20)
- Pak files can also be split into chunks for a bit of extra security
- Pak files are normally able to be viewed with [UEViewer](https://www.gildor.org/en/projects/umodel) or [Fmodel](https://fmodel.app/)
- Pak files can be extracted using tools such as the ones found in [Pakers/Unpakers](../Tools/Pakers.md)
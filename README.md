<h1 align="center">Backup</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.8-blue.svg" />
</p>

> This is a lightweight Python rsync wrapper for handling multiple locations to synchronize. It allows for automatization of backups to the currently available location pairs.

## Setup
After adding the binaries to your `$PATH`, you can set up your locations and Android phone paths in the `config/locations.json` and `config/cell.json` files.

The respective format for location pairs is:
```json
{
	"src":    "source path",
	"dst":    "destination path",
	"ignore": false
}
```
The source contents will be copied to the destination directory, given that `ignore` is set to `false`.

The `config/cell.json` contains an array of the Android folder paths.

## Usage
The `cellphone` executable then copies the contents of the specified Android folders to the current working directory.
The `backup` executable syncs the provided source and destination pairs.

## Author

👤 **Florian Schmidt**

* Website: [schmidt-allgaeu.de](https://schmidt-allgaeu.de)
* Github: [@flodt](https://github.com/flodt)

## Show your support

Give a ⭐️ if you like this project!

***
Built with ❤️ by Florian Schmidt.
# inno-setup-action

This action uses [Inno Setup](https://jrsoftware.org/isinfo.php) to create an installer for applications built as part of your GitHub Actions workflow.

## Inputs
#### `filepath`
**Required**
**Description** - Path to your ISS (Inno Setup Script) file

#### `options`
**Optional**
**Description** - Additional options to pass to Inno Setup

## Usage
Create your ISS file using Inno Setup, and add it to your repository.
After that, it can be used as part of your GitHub Actions workflow.

```
      - name: Run Inno Setup
        uses: robin24/inno-setup-action@v1
        with:
          filepath: ./sim-cpdlc.iss
          options: /O+
```

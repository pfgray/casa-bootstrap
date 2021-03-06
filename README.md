# CASA Bootstrap

The [Community App Sharing Architecture (CASA)](http://imsglobal.github.io/casa) provides a mechanism for
discovering and sharing metadata about web resources such as websites, mobile
apps and LTI tools. It models real-world decision-making through extensible
attributes, filter and transform operations, flexible peering relationships,
etc.

This is a bootstrapper for the CASA reference implementation.

## License

This software is **open-source** and licensed under the Apache 2 license.
The full text of the license may be found in the `LICENSE` file.

## Usage

### Development Environment

The environment may be downloaded and setup with the following command:

```
curl -L -0 http://imsglobal.github.io/casa-bootstrap/local | sh -s
```

This will create a `casa` directory with a number of locally linked gem repositories underneath.

The next thing that one must do is configure the gems they wish to run. This can be done by hand or with the `casa-environment` gem. To use the latter, navigate to `casa/casa-environment`. From within this directory, edit `config/local.json` and then call the `casa-environment configure` command on it.

```
cd casa/casa-environment
bundle exec casa-environment configure
```

See [casa-environment](https://github.com/IMSGlobal/casa-environment) for more details.

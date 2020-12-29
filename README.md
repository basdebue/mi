# mi

**`mi`** (short for **miles**) is a running calculator for the terminal. Given two of the three variables of distance, pace and time, `mi` will calculate the third and format the data as a nice table.

```sh
$ mi -d 10km -p 3:35/km
distance 10.00km
    time 35:50
    pace 3:35/km
   speed 16.7km/h
```

Distance, pace and time are passed using the `-d`, `-p` and `-t` options respectively. Supported units include MM:SS, kilometers, miles and all combinations thereof. Speed, expressed in either km/h or mph, can be used instead of pace. As `mi` is written in portable, POSIX-compliant sh, it does *not* support GNU-style long options à la `--distance`.

By default, `mi` will attempt to use your configured locale to determine your preferred measurement unit. If this doesn't work or doesn't pick the appropriate unit, you can set the `MI_UNITS` environment variable to `SI` or `IMPERIAL` for SI/metric units (kilometers) or imperial/U.S. customary units (miles) respectively.

## License

This project is licensed under the [ISC license](LICENSE). Any contribution intentionally submitted for inclusion by you shall also be licensed as such, without any additional terms or conditions.

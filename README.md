# Camo
[Camo](https://github.com/atmos/camo) is all about making insecure assets look secure. This is an SSL image proxy to prevent mixed content warnings on secure pages served.

# Getting started
1. Copy the `docker-compose.yml` to the server (only when not running local)
2. Put a strong shared secret key in `.env`

  ```
  CAMO_KEY=<strong shared secret key>
  ```

3. `docker-compose up -d`
4. Make sure all consumers of `camo` use the shared secret key to create their camofied image urls
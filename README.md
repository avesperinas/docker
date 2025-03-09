# Pushing New Docker Images

To push a new Docker image to GitHub Container Registry (GHCR), follow these steps:

**For new images:**

Create a new folder and Define the `Dockerfile`.

   ```sh
   mkdir -p docker/<image_name>
   touch docker/<image_name>/Dockerfile
   ```

**Push the changes to the registry:**  
   ```sh
   git add docker/<image_name>/Dockerfile
   git commit -m "<image_name>:X.Y.Z"
   git push origin master
   ```

This will trigger the CI pipeline, which will build and push the image to GHCR.   Make sure the commit message follows the given format.

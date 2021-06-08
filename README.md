**IMPORTANT**

I have not yet managed to get this working quite yet. Remaining tasks include:

- [ ] Writing our own PETSc and petsc4py `package.py` files
- [ ] Updating Firedrake and PyOP2 so they don't make breaking assumptions about being installed using the default `firedrake-install` script
- [ ] Determining a sensible way to permit updating packages without concrete version numbers (`spack develop` is the likely candidate)

---

To add this repository to spack run (from the repository root)

```bash
$ spack repo add .
```

## Using the Firedrake fork of PETSc

To get PETSc to clone from the Firedrake fork we apply a patch to the upstream `package.py` file from Spack.
To regenerate the `package.py` in this repository run the `rebase-petsc` script.

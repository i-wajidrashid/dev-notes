# Reading Log

1. [Python Virtual Environments and Packages](https://docs.python.org/3/tutorial/venv.html) - Isolating project dependencies with `venv` prevents package version conflicts across the host system.
2. [Django Deployment Checklist](https://docs.djangoproject.com/en/stable/howto/deployment/checklist/) - Disabling `DEBUG` and configuring `ALLOWED_HOSTS` are critical before exposing a Django app to production traffic.
3. [Google SRE: Eliminating Toil](https://sre.google/sre-book/eliminating-toil/) - Repetitive manual operational tasks should be automated so engineering time goes toward long-term system reliability.
4. [Ubuntu Security Notices (USN)](https://ubuntu.com/security/notices) - Monitoring USN advisories highlights which patched CVEs require immediate package upgrades on Ubuntu servers.
5. [GitHub Changelog](https://github.blog/changelog/) - Branch protection rules and required pull request reviews prevent untested code from being pushed directly to `main`.
6. [The Twelve-Factor App: Config](https://12factor.net/config) - Storing configuration and credentials in environment variables keeps secrets strictly separated from version-controlled code.
7. [Django Database Access Optimization](https://docs.djangoproject.com/en/stable/topics/db/optimization/) - Using `select_related` and `prefetch_related` eliminates the N+1 query bottleneck in Django ORM lookups.
8. [Understanding the Python GIL](https://realpython.com/python-gil/) - Because the Global Interpreter Lock limits execution to one thread at a time, CPU-bound workloads need `multiprocessing` instead of `threading`.
9. [Docker Multi-Stage Builds](https://docs.docker.com/build/building/multi-stage/) - Multi-stage Dockerfiles strip out build dependencies to shrink production container size and reduce the attack surface.
10. [Ubuntu OpenSSH Server Security](https://ubuntu.com/server/docs/security-openssh) - Disabling password authentication in favor of SSH keys blocks automated brute-force login attempts.

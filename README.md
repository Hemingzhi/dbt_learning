# dbt_learning

This repository is used to share the learning progress of Mingzhi on `dbt`.


## ⚠️ dbt Profile Configuration Options
| Method                                  | Bundled with Project | Recommended Usage               | How to Use                                                         |
| --------------------------------------- | -------------------- | ------------------------------- | ------------------------------------------------------------------ |
| Default `~/.dbt/profiles.yml`           | ❌ No                 | Local individual development    | Manually create the file under `~/.dbt/` and configure connection. |
| `--profiles-dir` (project-relative)     | ✅ Yes                | Team collaboration, cloud setup | Run dbt with `--profiles-dir ./profiles` from the project root.    |
| `DBT_PROFILES_DIR` environment variable | ✅ Yes                | Automation, Docker, CI/CD       | Set `export DBT_PROFILES_DIR=/path/to/your/project/profiles`.      |

Choose the option that best fits your environment and workflow. Using a project-level profiles/ directory is ideal for sharing consistent configurations with others.
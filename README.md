# CVMFS Catalog Visualizations

Interactive sunburst charts showing the catalog hierarchy and download costs for CERN CVMFS repositories.

**Live site:** https://chrisburr.github.io/cvmfs-catalog-visualizations/

## How it works

A GitHub Actions workflow runs weekly to:
1. Clone [python-cvmfsutils](https://github.com/chrisburr/python-cvmfsutils) (dev branch)
2. Run `catalog_visualizer` for each CVMFS repository
3. Deploy generated HTML files to GitHub Pages

Each repository is processed independently - failures don't affect other repos.

## Manual trigger

Go to Actions > "Generate CVMFS Catalog Visualizations" > "Run workflow"

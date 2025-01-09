deploy:
    needs: build
    permissions:
      pages: write
      id-token: write
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    steps:
    - name: Configure Pages
      uses: actions/configure-pages@v4
    - name: Deploy to GitHub Pages
      id: deployment
      uses: actions/deploy-pages@v4

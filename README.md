

# Build pages with:

```

# 1. build with specific base path
npx astro build --base /MedDok-site/build_1
npx astro build --base /MedDok-site/build_2


# 2. fix logo
grep -rlE '[^a-zA-Z0-9_]/logo\.jpg' build_2 | xargs sed -i '' -E 's#([^a-zA-Z0-9_])/logo\.jpg#\1/MedDok-site/build_2/logo.jpg#g'

```





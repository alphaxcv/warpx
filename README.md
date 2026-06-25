# warp-on-actions

```
      - name: Set up WARP
        uses: alphaxcv/warpx@1.0
```

```
      - name: Run renew
        run: |
          xvfb-run -a --server-args="-screen 0 1920x1080x24" bash -c \
          'sudo ip netns exec warp env DISPLAY="$DISPLAY" PYTHONUNBUFFERED=1 python -u renew.py'
```

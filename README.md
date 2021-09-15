# Proxy_Wifi_Check
偵測是否有開啟proxy代理伺服器


 private boolean isWifiProxy() {
        String proxyAddress = System.getProperty("http.proxyHost");
        String portStr = System.getProperty("http.proxyPort");
        int proxyPort = Integer.parseInt(portStr != null ? portStr : "-1");
        return !TextUtils.isEmpty(proxyAddress) && proxyPort != -1;
    }

# helloworld
this is another hello world project

# history
https://github.com/search?q=import+org.apache.log4j+HttpServletRequest&type=Code
<br/>
https://github.com/search?q=getHeaderNames+org.apache.log4j.Logger&type=Code
<br/>
https://github.com/search?q=+%27.debug%28req%27+log4j+HttpServletRequest&type=Code
<br/>
https://github.com/search?q=+%27.debug%28HttpServletRequest%27+%27org.apache.log4j%27&type=Code


# 123456789 :
https://github.com/zanni/messaging-server/blob/07372443224edfc75567c800a6781030cf33a730/backend-rabbitmq/src/main/java/com/bzanni/messagingserver/config/HttpRequestLoggingFilter.java<br/>
<code>LOGGER.debug(req.getRemoteHost() + " - " + req.getMethod() + " - " + res.getStatus() + " - " + req.getRequestURI());</code><br/>
<hr/>
https://github.com/jedibig/BankingApplication_ver2/blob/d40825938bfe9a75bf154bcdbe6de2e91f28d9a3/BankingApp_ver2/src/com/java/filter/RegistrationAuthentication.java<br/>
<code>@WebFilter("/account/*")</code><br/>
<code>logger.info("Response generated for url " + req.getRequestURI());</code>
<hr/>
https://github.com/prod-dev/travel/blob/7161d49bf3efbe57b67ac192f1f7fc5eb606f0cc/src/main/java/com/travel/filter/LogFilter.java<br/>
<code>HttpServletRequest req = (HttpServletRequest) request;</code><br>
<code>String queryString = req.getQueryString() == null ? "" : req.getQueryString();</code><br>
<code>LOG.debug("==" + req.getScheme() + "://" + req.getServerName() + req.getRequestURI() + queryString);</code><br>
<hr/>
https://github.com/VitaliiLysenko-cpu/Payments/blob/50dde6a3596dbb3649ff5c96999ef031f2404dde/src/main/java/com/lysenko/payments/servlet/account/TopUpAccountServlet.java<br/>
<code>String tot = req.getParameter("total");</code><br/>
<code>log.debug("total :" + tot);</code><br/>
<hr/>
https://github.com/edu-sharing/Edu-Sharing/blob/2c92708f0cd51fe990024beada09e263ce853018/Backend/src/org/edu_sharing/repository/server/PreviewServlet.java<br/>
<code>private boolean handleExternalThumbnail(HttpServletRequest req, HttpServletResponse resp, String url) throws IOException {</code><br/>
<code>if ("false".equalsIgnoreCase(req.getParameter("allowRedirect")) &&</code><br/>
<code>LightbendConfigLoader.get().getStringList("repository.communication.preview.remoteAllowList").stream().anyMatch((reg) -> {</code><br/>
<code>Pattern pattern = Pattern.compile(reg);</code><br/>
<code>Matcher matched = pattern.matcher(url);</code><br/>
<code>return matched.matches();</code><br/>
<code>})) {</code><br/>
<code>logger.debug("Follow redirect allowed for " + url);</code><br/>
<code>try(InputStream is = new HttpQueryTool().getStream(url)) {</code><br/>
<code>resp.setHeader("Content-Type", "image/jpeg");</code><br/>
<code>StreamUtils.copy(is, resp.getOutputStream());</code><br/>
<code>return true;</code><br/>
<code>} catch(Throwable t) {</code><br/>
<code>logger.info("Fetching preview via http failed for: " + url, t);</code><br/>
<code>}</code><br/>
<code>}</code><br/>
<code>resp.sendRedirect(url);</code><br/>
<code>return true;</code><br/>
<code>}</code><br/>

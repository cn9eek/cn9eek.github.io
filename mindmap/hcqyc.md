  <script src="map.js"></script>
<div id="main-area">
      <div id="content-info">
        <div id="content-info">
          <div id="title">缓冲区溢出攻击及防御技术</div>
        </div>
      </div>
      <div id="main-content">
        <div id="svg-container"><svg xmlns:ev="http://www.w3.org/2001/xml-events" width="2187" viewBox="0 0 2187 1537" ed:vSpacing="30" xmlns="http://www.w3.org/2000/svg" ed:name="Page-1" preserveAspectRadio="xMinYMin meet" xmlns:xlink="http://www.w3.org/1999/xlink" ed:hSpacing="30" height="1537" xmlns:ed="http://www.edrawsoft.cn/xml/2017/SVGExtensions/" id="page1">
    <style type="text/css"><![CDATA[
g[ed\:togtopicid],g[ed\:hyperlink],g[ed\:comment],g[ed\:note] {cursor:pointer;}
svg text::selection,svg tspan::selection{background-color: #4285f4;color: #ffffff;fill: #ffffff;}
.st52 {fill:#000000;font-family:Open Sans;font-size:10pt}
.st51 {fill:#303030;font-family:Open Sans;font-size:13pt}
.st50 {fill:#4c4c4c;font-family:Open Sans;font-size:18pt;font-weight:bold}
]]></style>
    <defs>
        <linearGradient x1="0%" y2="100%" y1="0%" x2="0%" id="lg17">
            <stop offset="0" stop-color="#ffffff"/>
            <stop offset="0.25" stop-color="#f0f5f0"/>
            <stop offset="0.75" stop-color="#e1ebe1"/>
            <stop offset="1" stop-color="#c8d7c8"/>
        </linearGradient>
    </defs>
    <rect width="2187" x="0" height="1537" fill="#ffffff" y="0"/>
    <path d="M54.2,0L82.3,0C82.3,0,84.9,0,88.3,0L117.3,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="103" transform="matrix(1,0,0,1,1312,768)" ed:tosuperid="102"/>
    <path d="M-13.5,76.6L3.7,76.6L3.7,-70.6C3.7,-73.9,6.4,-76.6,9.7,-76.6L13.5,-76.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="102" fill="none" id="105" transform="matrix(1,0,0,1,1516,691)" ed:tosuperid="104"/>
    <path d="M-13.5,16.5L3.7,16.5L3.7,-10.5C3.7,-13.8,6.4,-16.5,9.7,-16.5L13.5,-16.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="104" fill="none" id="107" transform="matrix(1,0,0,1,1639,598)" ed:tosuperid="106"/>
    <path d="M3.7,3C3.7,-0.3,6.4,-3,9.7,-3L13.5,-3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="104" fill="none" id="109" transform="matrix(1,0,0,1,1639,612)" ed:tosuperid="108"/>
    <path d="M3.7,-10.5L3.7,4.5C3.7,7.8,6.4,10.5,9.7,10.5L13.5,10.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="104" fill="none" id="111" transform="matrix(1,0,0,1,1639,625)" ed:tosuperid="110"/>
    <path d="M3.7,-24L3.7,18C3.7,21.3,6.4,24,9.7,24L13.5,24" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="104" fill="none" id="113" transform="matrix(1,0,0,1,1639,639)" ed:tosuperid="112"/>
    <path d="M3.7,31.6L3.7,-25.6C3.7,-28.9,6.4,-31.6,9.7,-31.6L13.5,-31.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="102" fill="none" id="115" transform="matrix(1,0,0,1,1516,736)" ed:tosuperid="114"/>
    <path d="M3.7,10.6L3.7,-4.6C3.7,-7.9,6.4,-10.6,9.7,-10.6L13.5,-10.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="102" fill="none" id="117" transform="matrix(1,0,0,1,1516,757)" ed:tosuperid="116"/>
    <path d="M3.7,-2.9C3.7,0.3,6.4,2.9,9.7,2.9L13.5,2.9" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="102" fill="none" id="119" transform="matrix(1,0,0,1,1516,771)" ed:tosuperid="118"/>
    <path d="M3.7,-23.1L3.7,17.1C3.7,20.4,6.4,23.1,9.7,23.1L13.5,23.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="102" fill="none" id="121" transform="matrix(1,0,0,1,1516,791)" ed:tosuperid="120"/>
    <path d="M-13.5,6.8L3.7,6.8L3.7,-0.8C3.7,-4.1,6.4,-6.8,9.7,-6.8L13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="120" fill="none" id="123" transform="matrix(1,0,0,1,1626,808)" ed:tosuperid="122"/>
    <path d="M3.7,-6.8L3.7,0.8C3.7,4.1,6.4,6.8,9.7,6.8L13.5,6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="120" fill="none" id="125" transform="matrix(1,0,0,1,1626,821)" ed:tosuperid="124"/>
    <path d="M3.7,-70.4L3.7,64.4C3.7,67.7,6.4,70.4,9.7,70.4L13.5,70.4" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="102" fill="none" id="127" transform="matrix(1,0,0,1,1516,838)" ed:tosuperid="126"/>
    <path d="M-13.5,27L3.7,27L3.7,-21C3.7,-24.3,6.4,-27,9.7,-27L13.5,-27" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="126" fill="none" id="129" transform="matrix(1,0,0,1,1639,882)" ed:tosuperid="128"/>
    <path d="M3.7,13.5L3.7,-7.5C3.7,-10.8,6.4,-13.5,9.7,-13.5L13.5,-13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="126" fill="none" id="131" transform="matrix(1,0,0,1,1639,895)" ed:tosuperid="130"/>
    <path d="M3.7,0C3.7,0,6.4,0,9.7,0L13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="126" fill="none" id="133" transform="matrix(1,0,0,1,1639,909)" ed:tosuperid="132"/>
    <path d="M3.7,-13.5L3.7,7.5C3.7,10.8,6.4,13.5,9.7,13.5L13.5,13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="126" fill="none" id="135" transform="matrix(1,0,0,1,1639,922)" ed:tosuperid="134"/>
    <path d="M3.7,-27L3.7,21C3.7,24.3,6.4,27,9.7,27L13.5,27" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="126" fill="none" id="137" transform="matrix(1,0,0,1,1639,936)" ed:tosuperid="136"/>
    <path d="M3.7,-110.9L3.7,104.9C3.7,108.2,6.4,110.9,9.7,110.9L13.5,110.9" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="102" fill="none" id="139" transform="matrix(1,0,0,1,1516,879)" ed:tosuperid="138"/>
    <path d="M-54.3,-344.4L-82.3,-344.4L-82.3,338.4C-82.3,341.7,-84.9,344.4,-88.3,344.4L-117.3,344.4" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="141" transform="matrix(1,0,0,1,1077,1112)" ed:tosuperid="140"/>
    <path d="M13.5,18.9L-3.7,18.9L-3.7,-12.9C-3.7,-16.2,-6.4,-18.9,-9.7,-18.9L-13.5,-18.9" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="140" fill="none" id="143" transform="matrix(1,0,0,1,874,1438)" ed:tosuperid="142"/>
    <path d="M-3.7,-11.9L-3.7,5.9C-3.7,9.2,-6.4,11.9,-9.7,11.9L-13.5,11.9" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="140" fill="none" id="145" transform="matrix(1,0,0,1,874,1469)" ed:tosuperid="144"/>
    <path d="M13.5,17.3L-3.7,17.3L-3.7,-11.3C-3.7,-14.6,-6.4,-17.3,-9.7,-17.3L-13.5,-17.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="144" fill="none" id="147" transform="matrix(1,0,0,1,686,1463)" ed:tosuperid="146"/>
    <path d="M-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="144" fill="none" id="149" transform="matrix(1,0,0,1,686,1481)" ed:tosuperid="148"/>
    <path d="M13.5,-3.8L-3.7,-3.8L-3.7,-2.3C-3.7,1.1,-6.4,3.8,-9.7,3.8L-13.5,3.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="148" fill="none" id="151" transform="matrix(1,0,0,1,589,1484)" ed:tosuperid="150"/>
    <path d="M-3.7,-17.3L-3.7,11.3C-3.7,14.6,-6.4,17.3,-9.7,17.3L-13.5,17.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="144" fill="none" id="153" transform="matrix(1,0,0,1,686,1498)" ed:tosuperid="152"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="152" fill="none" id="155" transform="matrix(1,0,0,1,563,1515)" ed:tosuperid="154"/>
    <path d="M-54.3,-290L-82.3,-290L-82.3,284C-82.3,287.3,-84.9,290,-88.3,290L-117.3,290" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="157" transform="matrix(1,0,0,1,1077,1058)" ed:tosuperid="156"/>
    <path d="M13.5,-5.1L-3.7,-5.1L-3.7,-0.9C-3.7,2.4,-6.4,5.1,-9.7,5.1L-13.5,5.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="156" fill="none" id="159" transform="matrix(1,0,0,1,857,1353)" ed:tosuperid="158"/>
    <path d="M-54.3,-256L-82.3,-256L-82.3,250C-82.3,253.3,-84.9,256,-88.3,256L-117.3,256" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="161" transform="matrix(1,0,0,1,1077,1024)" ed:tosuperid="160"/>
    <path d="M13.5,-5.1L-3.7,-5.1L-3.7,-0.9C-3.7,2.4,-6.4,5.1,-9.7,5.1L-13.5,5.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="160" fill="none" id="163" transform="matrix(1,0,0,1,874,1285)" ed:tosuperid="162"/>
    <path d="M-54.3,-158.1L-82.3,-158.1L-82.3,152.1C-82.3,155.4,-84.9,158.1,-88.3,158.1L-117.3,158.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="165" transform="matrix(1,0,0,1,1077,926)" ed:tosuperid="164"/>
    <path d="M13.5,62.4L-3.7,62.4L-3.7,-56.4C-3.7,-59.7,-6.4,-62.4,-9.7,-62.4L-13.5,-62.4" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="164" fill="none" id="167" transform="matrix(1,0,0,1,806,1022)" ed:tosuperid="166"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="166" fill="none" id="169" transform="matrix(1,0,0,1,698,960)" ed:tosuperid="168"/>
    <path d="M-3.7,42.1L-3.7,-36.1C-3.7,-39.4,-6.4,-42.1,-9.7,-42.1L-13.5,-42.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="164" fill="none" id="171" transform="matrix(1,0,0,1,806,1042)" ed:tosuperid="170"/>
    <path d="M13.5,6.8L-3.7,6.8L-3.7,-0.8C-3.7,-4.1,-6.4,-6.8,-9.7,-6.8L-13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="170" fill="none" id="173" transform="matrix(1,0,0,1,709,993)" ed:tosuperid="172"/>
    <path d="M-3.7,-6.8L-3.7,0.8C-3.7,4.1,-6.4,6.8,-9.7,6.8L-13.5,6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="170" fill="none" id="175" transform="matrix(1,0,0,1,709,1007)" ed:tosuperid="174"/>
    <path d="M-3.7,21.9L-3.7,-15.9C-3.7,-19.2,-6.4,-21.9,-9.7,-21.9L-13.5,-21.9" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="164" fill="none" id="177" transform="matrix(1,0,0,1,806,1062)" ed:tosuperid="176"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="176" fill="none" id="179" transform="matrix(1,0,0,1,709,1041)" ed:tosuperid="178"/>
    <path d="M-3.7,-32.1L-3.7,26.1C-3.7,29.4,-6.4,32.1,-9.7,32.1L-13.5,32.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="164" fill="none" id="181" transform="matrix(1,0,0,1,806,1116)" ed:tosuperid="180"/>
    <path d="M13.5,20.3L-3.7,20.3L-3.7,-14.3C-3.7,-17.6,-6.4,-20.3,-9.7,-20.3L-13.5,-20.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="180" fill="none" id="183" transform="matrix(1,0,0,1,735,1128)" ed:tosuperid="182"/>
    <path d="M13.5,20.3L-3.7,20.3L-3.7,-14.3C-3.7,-17.6,-6.4,-20.3,-9.7,-20.3L-13.5,-20.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="182" fill="none" id="185" transform="matrix(1,0,0,1,664,1088)" ed:tosuperid="184"/>
    <path d="M-3.7,6.8L-3.7,-0.8C-3.7,-4.1,-6.4,-6.8,-9.7,-6.8L-13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="182" fill="none" id="187" transform="matrix(1,0,0,1,664,1101)" ed:tosuperid="186"/>
    <path d="M-3.7,-6.8L-3.7,0.8C-3.7,4.1,-6.4,6.8,-9.7,6.8L-13.5,6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="182" fill="none" id="189" transform="matrix(1,0,0,1,664,1115)" ed:tosuperid="188"/>
    <path d="M-3.7,-20.3L-3.7,14.3C-3.7,17.6,-6.4,20.3,-9.7,20.3L-13.5,20.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="182" fill="none" id="191" transform="matrix(1,0,0,1,664,1128)" ed:tosuperid="190"/>
    <path d="M-3.7,-13.5L-3.7,7.5C-3.7,10.8,-6.4,13.5,-9.7,13.5L-13.5,13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="180" fill="none" id="193" transform="matrix(1,0,0,1,735,1162)" ed:tosuperid="192"/>
    <path d="M-3.7,-27L-3.7,21C-3.7,24.3,-6.4,27,-9.7,27L-13.5,27" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="180" fill="none" id="195" transform="matrix(1,0,0,1,735,1176)" ed:tosuperid="194"/>
    <path d="M-3.7,-40.5L-3.7,34.5C-3.7,37.8,-6.4,40.5,-9.7,40.5L-13.5,40.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="180" fill="none" id="197" transform="matrix(1,0,0,1,735,1189)" ed:tosuperid="196"/>
    <path d="M-54.3,78.3L-82.3,78.3L-82.3,-72.3C-82.3,-75.6,-84.9,-78.3,-88.3,-78.3L-117.3,-78.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="199" transform="matrix(1,0,0,1,1077,690)" ed:tosuperid="198"/>
    <path d="M13.5,76.3L-3.7,76.3L-3.7,-70.3C-3.7,-73.6,-6.4,-76.3,-9.7,-76.3L-13.5,-76.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="198" fill="none" id="201" transform="matrix(1,0,0,1,789,535)" ed:tosuperid="200"/>
    <path d="M13.5,60.8L-3.7,60.8L-3.7,-54.8C-3.7,-58.1,-6.4,-60.8,-9.7,-60.8L-13.5,-60.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="200" fill="none" id="203" transform="matrix(1,0,0,1,653,398)" ed:tosuperid="202"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="202" fill="none" id="205" transform="matrix(1,0,0,1,569,338)" ed:tosuperid="204"/>
    <path d="M-3.7,40.5L-3.7,-34.5C-3.7,-37.8,-6.4,-40.5,-9.7,-40.5L-13.5,-40.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="200" fill="none" id="207" transform="matrix(1,0,0,1,653,419)" ed:tosuperid="206"/>
    <path d="M13.5,6.8L-3.7,6.8L-3.7,-0.8C-3.7,-4.1,-6.4,-6.8,-9.7,-6.8L-13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="206" fill="none" id="209" transform="matrix(1,0,0,1,569,371)" ed:tosuperid="208"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="208" fill="none" id="211" transform="matrix(1,0,0,1,372,365)" ed:tosuperid="210"/>
    <path d="M-3.7,-6.8L-3.7,0.8C-3.7,4.1,-6.4,6.8,-9.7,6.8L-13.5,6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="206" fill="none" id="213" transform="matrix(1,0,0,1,569,385)" ed:tosuperid="212"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="212" fill="none" id="215" transform="matrix(1,0,0,1,379,392)" ed:tosuperid="214"/>
    <path d="M-3.7,-20.3L-3.7,14.3C-3.7,17.6,-6.4,20.3,-9.7,20.3L-13.5,20.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="200" fill="none" id="217" transform="matrix(1,0,0,1,653,479)" ed:tosuperid="216"/>
    <path d="M13.5,20.3L-3.7,20.3L-3.7,-14.3C-3.7,-17.6,-6.4,-20.3,-9.7,-20.3L-13.5,-20.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="216" fill="none" id="219" transform="matrix(1,0,0,1,569,479)" ed:tosuperid="218"/>
    <path d="M13.5,20.3L-3.7,20.3L-3.7,-14.3C-3.7,-17.6,-6.4,-20.3,-9.7,-20.3L-13.5,-20.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="218" fill="none" id="221" transform="matrix(1,0,0,1,511,439)" ed:tosuperid="220"/>
    <path d="M-3.7,6.8L-3.7,-0.8C-3.7,-4.1,-6.4,-6.8,-9.7,-6.8L-13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="218" fill="none" id="223" transform="matrix(1,0,0,1,511,452)" ed:tosuperid="222"/>
    <path d="M-3.7,-6.8L-3.7,0.8C-3.7,4.1,-6.4,6.8,-9.7,6.8L-13.5,6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="218" fill="none" id="225" transform="matrix(1,0,0,1,511,466)" ed:tosuperid="224"/>
    <path d="M-3.7,-20.3L-3.7,14.3C-3.7,17.6,-6.4,20.3,-9.7,20.3L-13.5,20.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="218" fill="none" id="227" transform="matrix(1,0,0,1,511,479)" ed:tosuperid="226"/>
    <path d="M-3.7,-27L-3.7,21C-3.7,24.3,-6.4,27,-9.7,27L-13.5,27" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="216" fill="none" id="229" transform="matrix(1,0,0,1,569,527)" ed:tosuperid="228"/>
    <path d="M13.5,13.5L-3.7,13.5L-3.7,-7.5C-3.7,-10.8,-6.4,-13.5,-9.7,-13.5L-13.5,-13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="228" fill="none" id="231" transform="matrix(1,0,0,1,511,540)" ed:tosuperid="230"/>
    <path d="M-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="228" fill="none" id="233" transform="matrix(1,0,0,1,511,554)" ed:tosuperid="232"/>
    <path d="M-3.7,-13.5L-3.7,7.5C-3.7,10.8,-6.4,13.5,-9.7,13.5L-13.5,13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="228" fill="none" id="235" transform="matrix(1,0,0,1,511,567)" ed:tosuperid="234"/>
    <path d="M-3.7,-11.5L-3.7,5.5C-3.7,8.8,-6.4,11.5,-9.7,11.5L-13.5,11.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="198" fill="none" id="237" transform="matrix(1,0,0,1,789,623)" ed:tosuperid="236"/>
    <path d="M13.5,6.8L-3.7,6.8L-3.7,-0.8C-3.7,-4.1,-6.4,-6.8,-9.7,-6.8L-13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="236" fill="none" id="239" transform="matrix(1,0,0,1,627,628)" ed:tosuperid="238"/>
    <path d="M13.5,6.8L-3.7,6.8L-3.7,-0.8C-3.7,-4.1,-6.4,-6.8,-9.7,-6.8L-13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="238" fill="none" id="241" transform="matrix(1,0,0,1,543,614)" ed:tosuperid="240"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="240" fill="none" id="243" transform="matrix(1,0,0,1,418,608)" ed:tosuperid="242"/>
    <path d="M-3.7,-6.8L-3.7,0.8C-3.7,4.1,-6.4,6.8,-9.7,6.8L-13.5,6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="238" fill="none" id="245" transform="matrix(1,0,0,1,543,628)" ed:tosuperid="244"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="244" fill="none" id="247" transform="matrix(1,0,0,1,405,635)" ed:tosuperid="246"/>
    <path d="M-3.7,-13.5L-3.7,7.5C-3.7,10.8,-6.4,13.5,-9.7,13.5L-13.5,13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="236" fill="none" id="249" transform="matrix(1,0,0,1,627,648)" ed:tosuperid="248"/>
    <path d="M-3.7,-38.5L-3.7,32.5C-3.7,35.8,-6.4,38.5,-9.7,38.5L-13.5,38.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="198" fill="none" id="251" transform="matrix(1,0,0,1,789,650)" ed:tosuperid="250"/>
    <path d="M-3.7,-59.5L-3.7,53.5C-3.7,56.8,-6.4,59.5,-9.7,59.5L-13.5,59.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="198" fill="none" id="253" transform="matrix(1,0,0,1,789,671)" ed:tosuperid="252"/>
    <path d="M13.5,-7.5L-3.7,-7.5L-3.7,1.5C-3.7,4.8,-6.4,7.5,-9.7,7.5L-13.5,7.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="252" fill="none" id="255" transform="matrix(1,0,0,1,705,738)" ed:tosuperid="254"/>
    <path d="M13.5,14.6L-3.7,14.6L-3.7,-8.6C-3.7,-11.9,-6.4,-14.6,-9.7,-14.6L-13.5,-14.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="254" fill="none" id="257" transform="matrix(1,0,0,1,164,731)" ed:tosuperid="256"/>
    <path d="M-3.7,1.1C-3.7,-0.1,-6.4,-1.1,-9.7,-1.1L-13.5,-1.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="254" fill="none" id="259" transform="matrix(1,0,0,1,164,744)" ed:tosuperid="258"/>
    <path d="M-3.7,-100.4L-3.7,94.4C-3.7,97.7,-6.4,100.4,-9.7,100.4L-13.5,100.4" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="198" fill="none" id="261" transform="matrix(1,0,0,1,789,712)" ed:tosuperid="260"/>
    <path d="M13.5,20.6L-3.7,20.6L-3.7,-14.6C-3.7,-17.9,-6.4,-20.6,-9.7,-20.6L-13.5,-20.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="260" fill="none" id="263" transform="matrix(1,0,0,1,705,792)" ed:tosuperid="262"/>
    <path d="M-3.7,-6.4L-3.7,0.4C-3.7,3.7,-6.4,6.4,-9.7,6.4L-13.5,6.4" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="260" fill="none" id="265" transform="matrix(1,0,0,1,705,819)" ed:tosuperid="264"/>
    <path d="M13.5,13.5L-3.7,13.5L-3.7,-7.5C-3.7,-10.8,-6.4,-13.5,-9.7,-13.5L-13.5,-13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="264" fill="none" id="267" transform="matrix(1,0,0,1,569,812)" ed:tosuperid="266"/>
    <path d="M-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="264" fill="none" id="269" transform="matrix(1,0,0,1,569,825)" ed:tosuperid="268"/>
    <path d="M-3.7,-13.5L-3.7,7.5C-3.7,10.8,-6.4,13.5,-9.7,13.5L-13.5,13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="264" fill="none" id="271" transform="matrix(1,0,0,1,569,839)" ed:tosuperid="270"/>
    <path d="M-3.7,-133.8L-3.7,127.8C-3.7,131.1,-6.4,133.8,-9.7,133.8L-13.5,133.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="198" fill="none" id="273" transform="matrix(1,0,0,1,789,745)" ed:tosuperid="272"/>
    <path d="M-3.7,-147.3L-3.7,141.3C-3.7,144.6,-6.4,147.3,-9.7,147.3L-13.5,147.3" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="198" fill="none" id="275" transform="matrix(1,0,0,1,789,759)" ed:tosuperid="274"/>
    <path d="M-54.3,260.6L-82.3,260.6L-82.3,-254.6C-82.3,-257.9,-84.9,-260.6,-88.3,-260.6L-117.3,-260.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="277" transform="matrix(1,0,0,1,1077,507)" ed:tosuperid="276"/>
    <path d="M13.5,8.4L-3.7,8.4L-3.7,-2.4C-3.7,-5.7,-6.4,-8.4,-9.7,-8.4L-13.5,-8.4" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="276" fill="none" id="279" transform="matrix(1,0,0,1,823,238)" ed:tosuperid="278"/>
    <path d="M-3.7,-5.1L-3.7,-0.9C-3.7,2.4,-6.4,5.1,-9.7,5.1L-13.5,5.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="276" fill="none" id="281" transform="matrix(1,0,0,1,823,252)" ed:tosuperid="280"/>
    <path d="M-3.7,-18.6L-3.7,12.6C-3.7,15.9,-6.4,18.6,-9.7,18.6L-13.5,18.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="276" fill="none" id="283" transform="matrix(1,0,0,1,823,265)" ed:tosuperid="282"/>
    <path d="M-54.3,334.6L-82.3,334.6L-82.3,-328.6C-82.3,-331.9,-84.9,-334.6,-88.3,-334.6L-117.3,-334.6" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="101" fill="none" id="285" transform="matrix(1,0,0,1,1077,433)" ed:tosuperid="284"/>
    <path d="M13.5,15.1L-3.7,15.1L-3.7,-9.1C-3.7,-12.4,-6.4,-15.1,-9.7,-15.1L-13.5,-15.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="284" fill="none" id="287" transform="matrix(1,0,0,1,789,84)" ed:tosuperid="286"/>
    <path d="M13.5,13.5L-3.7,13.5L-3.7,-7.5C-3.7,-10.8,-6.4,-13.5,-9.7,-13.5L-13.5,-13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="286" fill="none" id="289" transform="matrix(1,0,0,1,718,55)" ed:tosuperid="288"/>
    <path d="M-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="286" fill="none" id="291" transform="matrix(1,0,0,1,718,69)" ed:tosuperid="290"/>
    <path d="M-3.7,-13.5L-3.7,7.5C-3.7,10.8,-6.4,13.5,-9.7,13.5L-13.5,13.5" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="286" fill="none" id="293" transform="matrix(1,0,0,1,718,82)" ed:tosuperid="292"/>
    <path d="M-3.7,-11.9L-3.7,5.9C-3.7,9.2,-6.4,11.9,-9.7,11.9L-13.5,11.9" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="284" fill="none" id="295" transform="matrix(1,0,0,1,789,111)" ed:tosuperid="294"/>
    <path d="M13.5,0L-3.7,0C-3.7,0,-6.4,0,-9.7,0L-13.5,0" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="294" fill="none" id="297" transform="matrix(1,0,0,1,705,123)" ed:tosuperid="296"/>
    <path d="M-3.7,-32.1L-3.7,26.1C-3.7,29.4,-6.4,32.1,-9.7,32.1L-13.5,32.1" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="284" fill="none" id="299" transform="matrix(1,0,0,1,789,131)" ed:tosuperid="298"/>
    <path d="M13.5,6.8L-3.7,6.8L-3.7,-0.8C-3.7,-4.1,-6.4,-6.8,-9.7,-6.8L-13.5,-6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="298" fill="none" id="301" transform="matrix(1,0,0,1,705,156)" ed:tosuperid="300"/>
    <path d="M-3.7,-6.8L-3.7,0.8C-3.7,4.1,-6.4,6.8,-9.7,6.8L-13.5,6.8" stroke-linecap="round" stroke-linejoin="round" stroke="#4486b1" ed:parentid="298" fill="none" id="303" transform="matrix(1,0,0,1,705,170)" ed:tosuperid="302"/>
    <g ed:height="57" ed:topictype="mainidea" ed:layout="map" id="101" transform="matrix(1,0,0,1,1023,740)" ed:width="343">
        <path d="M4,0L339,0C341.2,0,343,1.8,343,4L343,53C343,55.2,341.2,57,339,57L4,57C1.8,57,0,55.2,0,53L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#000000" fill="#ffffff"/>
        <text class="st50">
            <tspan x="20" style="white-space:pre" y="37.8">缓冲区溢出攻击及防御技术</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="rightmap" ed:parentid="101" id="102" transform="matrix(1,0,0,1,1429,751)" ed:width="73">
        <path d="M4,0L69,0C71.2,0,73,1.8,73,4L73,31C73,33.2,71.2,35,69,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">防御</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="102" id="104" transform="matrix(1,0,0,1,1529,594)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">能被攻击原因</tspan>
        </text>
    </g>
    <g ed:height="35.5" ed:layout="rightmap" ed:parentid="104" id="106" transform="matrix(1,0,0,1,1652,546)" ed:width="514">
        <path d="M0,35.5L514,35.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">C语言对数据和指针不自动进行边界检测，一些字符串处理函数strcpy、sprintf等存</tspan>
            <tspan x="8" style="white-space:pre" y="29.4">在严重的安全问题</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="104" id="108" transform="matrix(1,0,0,1,1652,588)" ed:width="148">
        <path d="M0,20.5L148,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">程序员代码写的不严谨</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="104" id="110" transform="matrix(1,0,0,1,1652,615)" ed:width="330">
        <path d="M0,20.5L330,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">返回地址放在堆栈的底部，可以通过溢出覆盖放回地址</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="104" id="112" transform="matrix(1,0,0,1,1652,642)" ed:width="317">
        <path d="M0,20.5L317,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">堆栈的属性一般是可执行的，是的而已代码得意执行</tspan>
        </text>
    </g>
    <g ed:height="35.5" ed:layout="rightmap" ed:parentid="102" id="114" transform="matrix(1,0,0,1,1529,669)" ed:width="514">
        <path d="M0,35.5L514,35.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">提取用于攻击的shellcode的普遍特征作为攻击特征，过滤掉这样的数据包，或者触发</tspan>
            <tspan x="8" style="white-space:pre" y="29.4">报警</tspan>
        </text>
    </g>
    <g ed:height="35.5" ed:layout="rightmap" ed:parentid="102" id="116" transform="matrix(1,0,0,1,1529,711)" ed:width="514">
        <path d="M0,35.5L514,35.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">对特定的服务限定请求数据的值和范围，比如，某一服务器要求请求数据为可打印字符</tspan>
            <tspan x="8" style="white-space:pre" y="29.4">串，如果发现这一服务的请求存在不可打印字符则认为发生攻击</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="102" id="118" transform="matrix(1,0,0,1,1529,753)" ed:width="195">
        <path d="M0,20.5L195,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">源码BUG查找，使用安全的函数</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="102" id="120" transform="matrix(1,0,0,1,1529,794)" ed:width="83">
        <path d="M0,20.5L83,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">运行期保护</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="120" id="122" transform="matrix(1,0,0,1,1639,780)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">数据边界检查</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="120" id="124" transform="matrix(1,0,0,1,1639,807)" ed:width="148">
        <path d="M0,20.5L148,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">保证放回指针的完整性</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="102" id="126" transform="matrix(1,0,0,1,1529,888)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">加强系统保护</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="126" id="128" transform="matrix(1,0,0,1,1652,834)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">保护系统信息</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="126" id="130" transform="matrix(1,0,0,1,1652,861)" ed:width="122">
        <path d="M0,20.5L122,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">关闭不需要的服务</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="126" id="132" transform="matrix(1,0,0,1,1652,888)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">最小权限原则</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="126" id="134" transform="matrix(1,0,0,1,1652,915)" ed:width="135">
        <path d="M0,20.5L135,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">使用系统的堆栈补丁</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="126" id="136" transform="matrix(1,0,0,1,1652,942)" ed:width="187">
        <path d="M0,20.5L187,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">检查系统漏洞，及时打上补丁</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="rightmap" ed:parentid="102" id="138" transform="matrix(1,0,0,1,1529,969)" ed:width="161">
        <path d="M0,20.5L161,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">使用类型安全的语言开发</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="leftmap" ed:parentid="101" id="140" transform="matrix(1,0,0,1,887,1439)" ed:width="73">
        <path d="M4,0L69,0C71.2,0,73,1.8,73,4L73,31C73,33.2,71.2,35,69,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">方法</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="140" id="142" transform="matrix(1,0,0,1,660,1399)" ed:width="200">
        <path d="M0,20.5L200,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">在程序的地址空间安排适当代码</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="140" id="144" transform="matrix(1,0,0,1,699,1460)" ed:width="161">
        <path d="M0,20.5L161,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">使控制流跳转到攻击代码</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="144" id="146" transform="matrix(1,0,0,1,602,1426)" ed:width="70">
        <path d="M0,20.5L70,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">函数指针</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="144" id="148" transform="matrix(1,0,0,1,602,1460)" ed:width="70">
        <path d="M0,20.5L70,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">激活记录</tspan>
        </text>
    </g>
    <g ed:height="35.5" ed:layout="leftmap" ed:parentid="148" id="150" transform="matrix(1,0,0,1,61,1453)" ed:width="514">
        <path d="M0,35.5L514,35.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">当函数调用时，堆栈中会留驻一个Activation Record 包含函数返回的地址。溢出修</tspan>
            <tspan x="8" style="white-space:pre" y="29.4">改这一记录。</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="144" id="152" transform="matrix(1,0,0,1,576,1495)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">长跳转缓存区</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="152" id="154" transform="matrix(1,0,0,1,360,1495)" ed:width="189">
        <path d="M0,20.5L189,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">C语言的 setjmp 与 longjmp</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="leftmap" ed:parentid="101" id="156" transform="matrix(1,0,0,1,870,1331)" ed:width="90">
        <path d="M4,0L86,0C88.2,0,90,1.8,90,4L90,31C90,33.2,88.2,35,86,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">缓冲区</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="156" id="158" transform="matrix(1,0,0,1,461,1338)" ed:width="382">
        <path d="M0,20.5L382,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">相同数据类型实例的一个连续的计算机内存块，用于保存数据。</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="leftmap" ed:parentid="101" id="160" transform="matrix(1,0,0,1,887,1263)" ed:width="73">
        <path d="M4,0L69,0C71.2,0,73,1.8,73,4L73,31C73,33.2,71.2,35,69,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">溢出</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="160" id="162" transform="matrix(1,0,0,1,660,1270)" ed:width="200">
        <path d="M0,20.5L200,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">所填充的数据超出了原有的边界</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="leftmap" ed:parentid="101" id="164" transform="matrix(1,0,0,1,819,1067)" ed:width="141">
        <path d="M4,0L137,0C139.2,0,141,1.8,141,4L141,31C141,33.2,139.2,35,137,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">代码植入技术</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="164" id="166" transform="matrix(1,0,0,1,711,939)" ed:width="81">
        <path d="M0,20.5L81,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">shellcode</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="166" id="168" transform="matrix(1,0,0,1,432,939)" ed:width="252">
        <path d="M0,20.5L252,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">核心部分，能完成特殊任务的二进制代码</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="164" id="170" transform="matrix(1,0,0,1,722,980)" ed:width="70">
        <path d="M0,20.5L70,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">返回地址</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="170" id="172" transform="matrix(1,0,0,1,549,966)" ed:width="146">
        <path d="M0,20.5L146,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">shellcode的入口地址</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="170" id="174" transform="matrix(1,0,0,1,406,993)" ed:width="289">
        <path d="M0,20.5L289,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">设法用shellcode的入口地址覆盖某个跳转指令</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="164" id="176" transform="matrix(1,0,0,1,722,1020)" ed:width="70">
        <path d="M0,20.5L70,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">填充数据</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="176" id="178" transform="matrix(1,0,0,1,380,1020)" ed:width="315">
        <path d="M0,20.5L315,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">提高shellcode命中率，在前面安排一定的填充数据</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="164" id="180" transform="matrix(1,0,0,1,748,1128)" ed:width="44">
        <path d="M0,20.5L44,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">模式</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="180" id="182" transform="matrix(1,0,0,1,677,1088)" ed:width="44">
        <path d="M0,20.5L44,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">参数</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="182" id="184" transform="matrix(1,0,0,1,522,1047)" ed:width="128">
        <path d="M0,20.5L128,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">S 代表 Shellcode</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="182" id="186" transform="matrix(1,0,0,1,540,1074)" ed:width="110">
        <path d="M0,20.5L110,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">R 代表返回地址</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="182" id="188" transform="matrix(1,0,0,1,540,1101)" ed:width="110">
        <path d="M0,20.5L110,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">N 代表填充数据</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="182" id="190" transform="matrix(1,0,0,1,540,1128)" ed:width="110">
        <path d="M0,20.5L110,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">A 代表环境变量</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="180" id="192" transform="matrix(1,0,0,1,682,1155)" ed:width="39">
        <path d="M0,20.5L39,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">NSR</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="180" id="194" transform="matrix(1,0,0,1,682,1182)" ed:width="39">
        <path d="M0,20.5L39,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">RNS</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="180" id="196" transform="matrix(1,0,0,1,689,1209)" ed:width="32">
        <path d="M0,20.5L32,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">AR</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="leftmap" ed:parentid="101" id="198" transform="matrix(1,0,0,1,802,594)" ed:width="158">
        <path d="M4,0L154,0C156.2,0,158,1.8,158,4L158,31C158,33.2,156.2,35,154,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">缓冲区溢出原理</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="198" id="200" transform="matrix(1,0,0,1,666,439)" ed:width="109">
        <path d="M0,20.5L109,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">一段连续内存块</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="200" id="202" transform="matrix(1,0,0,1,582,317)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">代码段</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="202" id="204" transform="matrix(1,0,0,1,225,317)" ed:width="330">
        <path d="M0,20.5L330,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">存放程序的机器码和只读数据，可执行指令从这里取得</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="200" id="206" transform="matrix(1,0,0,1,582,358)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">数据段</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="206" id="208" transform="matrix(1,0,0,1,385,344)" ed:width="170">
        <path d="M0,20.5L170,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">以初始化的数据（.data）</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="208" id="210" transform="matrix(1,0,0,1,158,344)" ed:width="200">
        <path d="M0,20.5L200,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">保存全局和静态已初始化的变量</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="206" id="212" transform="matrix(1,0,0,1,392,371)" ed:width="163">
        <path d="M0,20.5L163,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">未初始化的数据（.bss）</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="212" id="214" transform="matrix(1,0,0,1,191,371)" ed:width="174">
        <path d="M0,20.5L174,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">全局和静态未初始化的变量</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="200" id="216" transform="matrix(1,0,0,1,582,479)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">堆栈端</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="216" id="218" transform="matrix(1,0,0,1,524,439)" ed:width="31">
        <path d="M0,20.5L31,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">堆</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="218" id="220" transform="matrix(1,0,0,1,185,398)" ed:width="312">
        <path d="M0,20.5L312,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">位于BBS内存段的上边，用来存储运行时分配的变量</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="218" id="222" transform="matrix(1,0,0,1,388,425)" ed:width="109">
        <path d="M0,20.5L109,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">动态扩张或缩减</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="218" id="224" transform="matrix(1,0,0,1,349,452)" ed:width="148">
        <path d="M0,20.5L148,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">malloc()、new()创建</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="218" id="226" transform="matrix(1,0,0,1,397,479)" ed:width="100">
        <path d="M0,20.5L100,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">delete()删除</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="216" id="228" transform="matrix(1,0,0,1,524,533)" ed:width="31">
        <path d="M0,20.5L31,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">栈</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="228" id="230" transform="matrix(1,0,0,1,310,506)" ed:width="187">
        <path d="M0,20.5L187,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">存储函数调用时临时信息结构</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="228" id="232" transform="matrix(1,0,0,1,206,533)" ed:width="291">
        <path d="M0,20.5L291,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">编译器需要的时候分配，不需要的时候自动清除</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="228" id="234" transform="matrix(1,0,0,1,401,560)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">先进后出队列</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="198" id="236" transform="matrix(1,0,0,1,640,614)" ed:width="135">
        <path d="M0,20.5L135,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">关注数据区和堆栈区</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="236" id="238" transform="matrix(1,0,0,1,556,601)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">使用栈</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="238" id="240" transform="matrix(1,0,0,1,431,587)" ed:width="98">
        <path d="M0,20.5L98,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">ESP 栈顶指针</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="240" id="242" transform="matrix(1,0,0,1,230,587)" ed:width="174">
        <path d="M0,20.5L174,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">随着数据入栈出栈发生变化</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="238" id="244" transform="matrix(1,0,0,1,418,614)" ed:width="111">
        <path d="M0,20.5L111,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">EBP 基地址指针</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="244" id="246" transform="matrix(1,0,0,1,21,614)" ed:width="370">
        <path d="M0,20.5L370,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">通过BP加上偏移地址，可以方便的引用函数参数已经局部变量</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="236" id="248" transform="matrix(1,0,0,1,228,641)" ed:width="385">
        <path d="M0,20.5L385,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">局部变量发生溢出，很有可能会覆盖掉EBP设置RET（返回地址）</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="198" id="250" transform="matrix(1,0,0,1,471,668)" ed:width="304">
        <path d="M0,20.5L304,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">在堆栈中压入的数据超过预先给堆栈分配的容量。</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="198" id="252" transform="matrix(1,0,0,1,718,710)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">栈溢出</tspan>
        </text>
    </g>
    <g ed:height="50.5" ed:layout="leftmap" ed:parentid="252" id="254" transform="matrix(1,0,0,1,177,695)" ed:width="514">
        <path d="M0,50.5L514,50.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">首先把指令寄存器（CPU要执行的下一条指令地址）压入栈，作为程序的返回地址</tspan>
            <tspan x="8" style="white-space:pre" y="29.4">（RET），之后作为栈的基址寄存器（EBP）它指向当前函数栈针的地步，而后把当前</tspan>
            <tspan x="8" style="white-space:pre" y="44.5">的栈顶指针，ESP拷贝到EBP基址寄存器，作为新的基地址。</tspan>
        </text>
    </g>
    <g ed:height="19" ed:layout="leftmap" ed:parentid="254" id="256" transform="matrix(1,0,0,1,121,697)" ed:width="29.5">
        <path d="M0,19L29.5,19" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="254" id="258" transform="matrix(1,0,0,1,80,723)" ed:width="70">
        <path d="M0,20.5L70,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">思维导图</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="198" id="260" transform="matrix(1,0,0,1,718,792)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">堆溢出</tspan>
        </text>
    </g>
    <g ed:height="19" ed:layout="leftmap" ed:parentid="260" id="262" transform="matrix(1,0,0,1,662,752)" ed:width="29.5">
        <path d="M0,19L29.5,19" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="260" id="264" transform="matrix(1,0,0,1,582,805)" ed:width="109">
        <path d="M0,20.5L109,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">不如栈溢出流行</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="264" id="266" transform="matrix(1,0,0,1,433,778)" ed:width="122">
        <path d="M0,20.5L122,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">比栈溢出难度更大</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="264" id="268" transform="matrix(1,0,0,1,433,805)" ed:width="122">
        <path d="M0,20.5L122,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">需要结合其他技术</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="264" id="270" transform="matrix(1,0,0,1,303,832)" ed:width="252">
        <path d="M0,20.5L252,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">对于内存中变量的组织方式有一定的要求</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="198" id="272" transform="matrix(1,0,0,1,710,859)" ed:width="65">
        <path d="M0,20.5L65,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">BBS溢出</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="198" id="274" transform="matrix(1,0,0,1,679,886)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">格式化串溢出</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="leftmap" ed:parentid="101" id="276" transform="matrix(1,0,0,1,836,229)" ed:width="124">
        <path d="M4,0L120,0C122.2,0,124,1.8,124,4L124,31C124,33.2,122.2,35,120,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">攻击三部曲</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="276" id="278" transform="matrix(1,0,0,1,468,210)" ed:width="341">
        <path d="M0,20.5L341,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">构造需要运行的shellcode，并将其放到目标系统的内存</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="276" id="280" transform="matrix(1,0,0,1,549,237)" ed:width="260">
        <path d="M0,20.5L260,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">获得缓存区的大小和定位溢出点RET的位置</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="276" id="282" transform="matrix(1,0,0,1,622,264)" ed:width="187">
        <path d="M0,20.5L187,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">控制程序跳转，改变程序流程</tspan>
        </text>
    </g>
    <g ed:height="35" ed:layout="leftmap" ed:parentid="101" id="284" transform="matrix(1,0,0,1,802,81)" ed:width="158">
        <path d="M4,0L154,0C156.2,0,158,1.8,158,4L158,31C158,33.2,156.2,35,154,35L4,35C1.8,35,0,33.2,0,31L0,4C0,1.8,1.8,0,4,0z" stroke-linejoin="round" stroke="#4486b1" fill="#ffffff"/>
        <text class="st51">
            <tspan x="18" style="white-space:pre" y="23.8">缓冲区溢出攻击</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="284" id="286" transform="matrix(1,0,0,1,731,48)" ed:width="44">
        <path d="M0,20.5L44,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">特点</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="286" id="288" transform="matrix(1,0,0,1,556,21)" ed:width="148">
        <path d="M0,20.5L148,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">不需要太多的先决条件</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="286" id="290" transform="matrix(1,0,0,1,621,48)" ed:width="83">
        <path d="M0,20.5L83,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">杀伤力很强</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="286" id="292" transform="matrix(1,0,0,1,634,75)" ed:width="70">
        <path d="M0,20.5L70,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">技术性强</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="284" id="294" transform="matrix(1,0,0,1,718,102)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">破坏性</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="294" id="296" transform="matrix(1,0,0,1,530,102)" ed:width="161">
        <path d="M0,20.5L161,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">极其容易使服务停止运行</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="284" id="298" transform="matrix(1,0,0,1,718,143)" ed:width="57">
        <path d="M0,20.5L57,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">隐蔽性</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="298" id="300" transform="matrix(1,0,0,1,543,129)" ed:width="148">
        <path d="M0,20.5L148,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">漏洞发现者并非编写者</tspan>
        </text>
    </g>
    <g ed:height="20.5" ed:layout="leftmap" ed:parentid="298" id="302" transform="matrix(1,0,0,1,595,156)" ed:width="96">
        <path d="M0,20.5L96,20.5" stroke-linejoin="round" stroke="#4486b1" fill="none"/>
        <text class="st52">
            <tspan x="8" style="white-space:pre" y="14.4">攻击代码很短</tspan>
        </text>
    </g>
    <symbol id="plus">
        <path d="M11,6C11,8.8,8.8,11,6,11C3.2,11,1,8.8,1,6C1,3.2,3.2,1,6,1C8.8,1,11,3.2,11,6z" fill="url(#lg17)"/>
        <path d="M11,6C11,8.8,8.8,11,6,11C3.2,11,1,8.8,1,6C1,3.2,3.2,1,6,1C8.8,1,11,3.2,11,6zM3,6L9,6M6,3L6,9" stroke="#46a000" fill="none" stroke-width="0.7"/>
    </symbol>
    <symbol id="minus">
        <path d="M11,6C11,8.8,8.8,11,6,11C3.2,11,1,8.8,1,6C1,3.2,3.2,1,6,1C8.8,1,11,3.2,11,6z" fill="url(#lg17)"/>
        <path d="M11,6C11,8.8,8.8,11,6,11C3.2,11,1,8.8,1,6C1,3.2,3.2,1,6,1C8.8,1,11,3.2,11,6zM3,6L9,6" stroke="#46a000" fill="none" stroke-width="0.7"/>
    </symbol>
    <g ed:togtopicid="101" transform="translate(1367,762)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="102" transform="translate(1503,762)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="104" transform="translate(1626,599)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="120" transform="translate(1613,798)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="126" transform="translate(1626,893)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="140" transform="translate(874,1451)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="144" transform="translate(686,1464)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="148" transform="translate(589,1464)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="152" transform="translate(563,1499)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="156" transform="translate(857,1342)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="160" transform="translate(874,1274)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="164" transform="translate(806,1078)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="166" transform="translate(698,943)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="170" transform="translate(709,984)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="176" transform="translate(709,1024)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="180" transform="translate(735,1132)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="182" transform="translate(664,1092)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="198" transform="translate(789,606)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="200" transform="translate(653,443)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="202" transform="translate(569,321)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="206" transform="translate(569,362)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="208" transform="translate(372,348)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="212" transform="translate(379,375)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="216" transform="translate(569,483)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="218" transform="translate(511,443)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="228" transform="translate(511,537)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="236" transform="translate(627,618)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="238" transform="translate(543,605)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="240" transform="translate(418,591)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="244" transform="translate(405,618)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="252" transform="translate(705,714)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="254" transform="translate(164,714)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="260" transform="translate(705,796)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="264" transform="translate(569,809)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="276" transform="translate(823,241)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="284" transform="translate(789,93)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="286" transform="translate(718,52)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="294" transform="translate(705,106)">
        <use xlink:href="#minus"/>
    </g>
    <g ed:togtopicid="298" transform="translate(705,147)">
        <use xlink:href="#minus"/>
    </g>
</svg>
</div>
      </div>
    </div>


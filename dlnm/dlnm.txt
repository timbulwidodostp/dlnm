# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Distributed lag linear and non-linear models (DLNM) for time series data Use crossbasis With (In) R Software
install.packages("dlnm")
library("dlnm")
dlnm = read.csv("https://raw.githubusercontent.com/timbulwidodostp/dlnm/main/dlnm/dlnm.csv",sep = ";")
# Estimation Distributed lag linear and non-linear models (DLNM) for time series data Use crossbasis With (In) R Software
dlnm_1 <- crossbasis(dlnm$pm10, lag=15, argvar=list(fun="lin"), arglag=list(fun="poly",degree=4))
summary(dlnm_1)
dlnm_2 <- crossbasis(dlnm$pm10, lag=1, argvar=list(fun="lin"), arglag=list(fun="strata"))
summary(dlnm_2)
# Distributed lag linear and non-linear models (DLNM) for time series data Use crossbasis With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
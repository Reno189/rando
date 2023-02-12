var _____WB$wombat$assign$function_____ = function(name) {
	return (self._wb_wombat && self._wb_wombat.local_init && self._wb_wombat.local_init(name)) || self[name];
};
if (!self.__WB_pmw) {
	self.__WB_pmw = function(obj) {
		this.__WB_source = obj;
		return this;
	}
} {
	let window = _____WB$wombat$assign$function_____("window");
	let self = _____WB$wombat$assign$function_____("self");
	let document = _____WB$wombat$assign$function_____("document");
	let location = _____WB$wombat$assign$function_____("location");
	let top = _____WB$wombat$assign$function_____("top");
	let parent = _____WB$wombat$assign$function_____("parent");
	let frames = _____WB$wombat$assign$function_____("frames");
	let opener = _____WB$wombat$assign$function_____("opener");

	! function(e) {
		function t(n) {
			if (a[n]) return a[n].exports;
			var s = a[n] = {
				exports: {},
				id: n,
				loaded: !1
			};
			return e[n].call(s.exports, s, s.exports, t), s.loaded = !0, s.exports
		}
		var a = {};
		return t.m = e, t.c = a, t.p = "/build/", t(0)
	}([function(e, t, a) {
		e.exports = a(23)
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = Object.assign || function(e) {
				for (var t = 1; t < arguments.length; t++) {
					var a = arguments[t];
					for (var n in a) Object.prototype.hasOwnProperty.call(a, n) && (e[n] = a[n])
				}
				return e
			},
			c = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			l = a(32),
			u = n(l),
			d = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						position_from_top: 0,
						is_mobile_navigation_active: !1
					}, n
				}
				return r(t, e), c(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.updatePositionFromTop(), window.addEventListener("scroll", _.debounce(this.updatePositionFromTop, 300, {
							leading: !0,
							trailing: !0
						}), !1), $(".tse-scrollable").TrackpadScrollEmulator({
							wrapContent: !0,
							audoHide: !0
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "updatePositionFromTop",
					value: function(e) {
						this.setState({
							position_from_top: $(window).scrollTop()
						})
					}
				}, {
					key: "toggleMobileNavigation",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.setState({
							is_mobile_navigation_active: !this.state.is_mobile_navigation_active
						}), !1
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: classNames(this.props.className, "header-container")
						}, React.createElement("div", {
							className: classNames("header", {
								"solid-bg": this.state.position_from_top > 0
							})
						}, React.createElement("div", {
							className: "mobile-header-nav-item clickable",
							onMouseDown: this.toggleMobileNavigation,
							onTouchStart: this.toggleMobileNavigation
						}, React.createElement("div", {
							id: "nav_hamburger",
							className: classNames({
								"animated-icon": !0,
								hamburger: !0,
								open: this.state.is_mobile_navigation_active
							})
						}, React.createElement("span", null), React.createElement("span", null), React.createElement("span", null), React.createElement("span", null), React.createElement("span", null), React.createElement("span", null))), React.createElement("a", {
							href: "/",
							className: "mobile-header-nav-item"
						}, React.createElement("img", {
							src: "/logo-100.png",
							alt: "Logo",
							className: "logo"
						}), "hanime.tv"), this.props.children, React.createElement("a", {
							href: "/",
							className: classNames({
								"header-nav-item": !0,
								active: "Landing" === this.props.layout
							})
						}, React.createElement("img", {
							src: "/logo-100.png",
							alt: "Logo",
							className: "logo"
						})), React.createElement("a", {
							href: "/search",
							className: classNames({
								"header-nav-item": !0,
								active: "Search" === this.props.layout
							})
						}, React.createElement("span", {
							className: "item"
						}, "Search")), React.createElement("a", {
							href: "/apps",
							className: classNames({
								"header-nav-item": !0,
								active: "Apps" === this.props.layout
							})
						}, React.createElement("span", {
							className: "item"
						}, "Apps")), this.props.current_user ? React.createElement("div", {
							className: "header-nav-item-group"
						}, React.createElement(u["default"], o({
							className: "header-nav-item"
						}, this.props))) : React.createElement("div", {
							className: "header-nav-item-group"
						}, React.createElement("a", {
							href: "/log-in",
							className: classNames({
								"header-nav-item": !0,
								active: "LogIn" === this.props.layout
							})
						}, "Login"), React.createElement("a", {
							href: "/create-account",
							className: classNames({
								"header-nav-item": !0,
								active: "SignUp" === this.props.layout
							})
						}, "Create Account"))), React.createElement("div", {
							className: classNames({
								"header-mobile-nav-bg": !0,
								active: this.state.is_mobile_navigation_active
							}),
							onClick: this.toggleMobileNavigation
						}), React.createElement("div", {
							className: classNames({
								"header-mobile-nav-panel": !0,
								"tse-scrollable": !0,
								active: this.state.is_mobile_navigation_active
							})
						}, React.createElement("div", {
							className: "tse-content"
						}, React.createElement("a", {
							href: "/",
							className: classNames({
								"header-mobile-nav-panel-item": !0,
								active: "Landing" === this.props.layout
							})
						}, React.createElement("span", {
							className: "item"
						}, "Home")), React.createElement("a", {
							href: "/search",
							className: classNames({
								"header-mobile-nav-panel-item": !0,
								active: "Search" === this.props.layout
							})
						}, React.createElement("span", {
							className: "item"
						}, "Search")), React.createElement("a", {
							href: "/apps",
							className: classNames({
								"header-mobile-nav-panel-item": !0,
								active: "Apps" === this.props.layout
							})
						}, React.createElement("span", {
							className: "item"
						}, "Apps")), React.createElement("a", {
							href: "https://web.archive.org/web/20170201123401/https://htvanime.com",
							className: "header-mobile-nav-panel-item",
							target: "_blank"
						}, React.createElement("span", {
							className: "item"
						}, "Anime")), React.createElement("div", {
							className: "divider"
						}), this.props.current_user ? React.createElement("div", null, _.map(this.props.user_dropdown_items, function(t, a) {
							return React.createElement("a", {
								href: t.url,
								className: classNames("header-mobile-nav-panel-item", {
									active: e.props.layout === t.text
								}),
								key: a
							}, t.text)
						})) : React.createElement("div", null, React.createElement("a", {
							href: "/log-in",
							className: classNames({
								"header-mobile-nav-panel-item": !0,
								active: "LogIn" === this.props.layout
							})
						}, "Login"), React.createElement("a", {
							href: "/create-account",
							className: classNames({
								"header-mobile-nav-panel-item": !0,
								active: "SignUp" === this.props.layout
							})
						}, "Create Account")))))
					}
				}]), t
			}(React.Component);
		t["default"] = d
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						active: !1
					}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						App.events.addListener("MODAL_ACTIVATE", function(t) {
							e.setState({
								active: !0
							})
						}), App.events.addListener("MODAL_DEACTIVATE", function() {
							e.setState({
								active: !1
							})
						})
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: classNames("callout-background", {
								active: this.state.active
							})
						})
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						is_modal_content_rendered: !1,
						type: "login-required-modal",
						enterClass: null,
						title: null,
						body: null,
						form: {
							email: "",
							message: "",
							current_url: "",
							window_width: null,
							window_height: null,
							is_h264_supported: null,
							is_webm_supported: null,
							video_player_msg: null
						},
						is_loading: !1,
						is_footer_visible: !0
					}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						App.events.addListener("MODAL_ACTIVATE", function(t) {
							e.setState({
								is_modal_content_rendered: !0,
								title: t.title || "",
								body: t.body || "",
								type: t.type,
								is_footer_visible: t.is_footer_visible || !0
							}, function() {
								setTimeout(function() {
									e.setState({
										enterClass: "enter"
									})
								}, 0)
							})
						}), App.events.addListener("MODAL_DEACTIVATE", function() {
							e.setState({
								enterClass: null
							})
						}), App.events.addListener("HTV_VIDEO_PLAYER_REPORTING", function(t) {
							var a = _.clone(e.state.form);
							_.each(t, function(e, t) {
								a[t] = e
							}), e.setState({
								form: a
							})
						})
					}
				}, {
					key: "closeModal",
					value: function() {
						App.events.emit("MODAL_DEACTIVATE")
					}
				}, {
					key: "isContactUsFormValid",
					value: function() {
						return 0 != this.state.form.message.length
					}
				}, {
					key: "reloadVideo",
					value: function(e) {
						e.preventDefault(), e.stopPropagation(), App.events.emit("HTV_VIDEO_PLAYER_RELOAD"), this.closeModal()
					}
				}, {
					key: "submitFeedback",
					value: function(e) {
						var t = this;
						if (e.preventDefault(), e.stopPropagation(), this.isContactUsFormValid() && !this.state.is_loading) {
							var a = _.clone(this.state.form);
							return a.current_url = window.location.href, a.window_width = $(window).width(), a.window_height = $(window).height(), this.setState({
								form: a,
								is_loading: !0
							}, function() {
								$.ajax({
									type: "POST",
									url: "/api/v1/feedbacks",
									data: {
										feedback: t.state.form
									},
									success: t.feedbackCreateResolved,
									error: t.feedbackCreateFailed
								})
							}), !1
						}
					}
				}, {
					key: "updateForm",
					value: function(e, t) {
						var a = this.state.form;
						a[t] = e.target.value, this.setState({
							form: a
						})
					}
				}, {
					key: "feedbackCreateResolved",
					value: function(e) {
						var t = this;
						this.setState({
							form: {
								email: "",
								message: "",
								current_url: ""
							},
							is_loading: !1,
							feedback_message: "Feedback sent!"
						}), $("#contact_us_form_body").val(""), setTimeout(function() {
							t.setState({
								feedback_message: null
							}), t.closeModal()
						}, 1500)
					}
				}, {
					key: "feedbackCreateFailed",
					value: function(e) {
						var t = this;
						console.error(e), this.setState({
							is_loading: !1,
							feedback_message: "Failed to send feedback."
						}), setTimeout(function() {
							t.setState({
								feedback_message: null
							})
						}, 1500)
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return this.state.is_modal_content_rendered ? React.createElement("div", null, this.state.is_modal_content_rendered ? React.createElement("div", {
							className: classNames("modal tse-scrollable", {
								hidden: !this.state.enterClass
							})
						}, React.createElement("div", {
							className: "modal-page-fill",
							onTouchStart: this.closeModal,
							onClick: this.closeModal
						}), React.createElement(ReactCSSTransitionGroup, {
							transitionName: "presenter",
							transitionAppearTimeout: 300,
							transitionEnterTimeout: 300,
							transitionLeaveTimeout: 300,
							className: "transition-group flex flex-row justify-center"
						}, this.state.enterClass ? React.createElement("div", {
							key: "unique",
							className: classNames("modal-content tse-content", "contact-us-modal" == this.state.type ? "contact-us" : "", this.state.enterClass)
						}, React.createElement("div", {
							className: classNames("modal-title", {
								active: this.state.title
							})
						}, React.createElement("div", {
							className: "title"
						}, this.state.title), React.createElement("div", {
							className: "close-icon",
							onTouchStart: this.closeModal,
							onClick: this.closeModal
						}, React.createElement("span", null, "×"))), "login-required-modal" == this.state.type || "warning-modal" == this.state.type || "video-player-error-modal" == this.state.type ? React.createElement("div", {
							className: "modal-body"
						}, React.createElement("div", {
							className: "body-text",
							dangerouslySetInnerHTML: {
								__html: this.state.body
							}
						})) : "contact-us-modal" == this.state.type ? React.createElement("div", {
							className: "modal-body contact-us"
						}, React.createElement("input", {
							className: "email inverse input-responsive",
							type: "email",
							placeholder: "Email (optional)",
							onChange: function(t) {
								e.updateForm(t, "email")
							}
						}), React.createElement("span", {
							className: "hint"
						}, "* Tip: If you ask us questions and don't put in your email, we can't answer you."), React.createElement("textarea", {
							id: "contact_us_form_body",
							className: "flex textarea-body inverse",
							onChange: function(t) {
								e.updateForm(t, "message")
							}
						})) : null, "login-required-modal" == this.state.type ? React.createElement("div", {
							className: "modal-footer"
						}, React.createElement("div", {
							className: "modal-footer-padding"
						}, React.createElement("div", {
							className: "button-container"
						}, React.createElement("a", {
							className: "btn btn-shadow",
							href: "/log-in"
						}, "Login"), React.createElement("a", {
							className: "btn btn-shadow flex",
							href: "/create-account"
						}, "Create a Free Account")))) : "contact-us-modal" == this.state.type ? React.createElement("div", {
							className: "modal-footer contact-us"
						}, React.createElement("div", {
							className: "modal-footer-padding"
						}, React.createElement("div", {
							className: "button-container"
						}, this.state.feedback_message ? React.createElement("div", null, this.state.feedback_message) : React.createElement("div", {
							className: "btn btn-shadow",
							onClick: this.submitFeedback,
							disabled: !this.isContactUsFormValid() || this.state.is_loading
						}, "Send")))) : "video-player-error-modal" == this.state.type ? React.createElement("div", {
							className: "modal-footer"
						}, React.createElement("div", {
							className: "modal-footer-padding"
						}, React.createElement("div", {
							className: "button-container"
						}, React.createElement("div", {
							className: "btn btn-shadow flex",
							onClick: this.reloadVideo
						}, "Reload Video")))) : null) : null)) : null) : null
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, 
	
	
	
	
	
	
	function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "shouldComponentUpdate",
					value: function(e, t) {
						return e.data && !this.props.data ? !0 : e.data.views != this.props.data.views ? !0 : e.data.favorites_count != this.props.data.favorites_count ? !0 : e.is_focused != this.props.is_focused ? !0 : e.data.cover_url != this.props.data.cover_url
					}
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: classNames(this.props.className, "card", {
								active: this.props.is_focused
							})
						}, React.createElement("div", {
							className: "outer"
						}, React.createElement("div", {
							className: "inner"
						}, React.createElement("div", {
							className: "card-content"
						}, React.createElement("div", {
							className: "cover"
						}, _.isEmpty(this.props.data) ? null : React.createElement("img", {
							className: classNames(this.props.is_load_image_immediately ? "" : "b-lazy b-lazy-pop-in", {
								faded: this.props.is_disabled
							}),
							src: this.props.is_load_image_immediately ? this.props.data.cover_url : App.transparent,
							"data-src": this.props.data.cover_url,
							width: "100%",
							height: "100%",
							alt: "Watch " + this.props.data.name + " Video"
						}), this.props.url_function ? React.createElement("a", {
							className: "details",
							href: this.props.url_function(this.props.data),
							onClick: function(t) {
								e.props.on_activate_function(t, e.props.url_function(e.props.data))
							}
						}, React.createElement("div", {
							className: "play-icon-container"
						}, React.createElement("em", {
							className: "play-icon fa fa-play"
						})), React.createElement("div", {
							className: "metadata"
						}, React.createElement("div", {
							className: "hint"
						}, _.isEmpty(this.props.data) ? "" : this.props.data.brand), React.createElement("div", {
							className: "title"
						}, _.isEmpty(this.props.data) ? "" : this.props.data.name), React.createElement("div", {
							className: "views"
						}, React.createElement("em", {
							className: "fa fa-eye"
						}), _.isEmpty(this.props.data) ? "" : this.props.data.views), this.props.addon ? this.props.addon(this.props.data) : null)) : null, this.props.is_disabled ? React.createElement("div", {
							className: "details disabled-details"
						}, React.createElement("div", {
							className: "play-icon-container"
						}), React.createElement("div", {
							className: "metadata"
						}, React.createElement("div", {
							className: "hint"
						}, _.isEmpty(this.props.data) ? "" : this.props.data.brand), React.createElement("div", {
							className: "title"
						}, React.createElement("div", {
							className: "here"
						}, "You Are Here"), _.isEmpty(this.props.data) ? "" : this.props.data.name), React.createElement("div", {
							className: "views"
						}, React.createElement("em", {
							className: "fa fa-eye"
						}), _.isEmpty(this.props.data) ? "" : this.props.data.views), this.props.addon ? this.props.addon(this.props.data) : null)) : null)))))
					}
				}
				
				
				
				
				
				
				
				
				
				
				
				]), t
			}(React.Component);
		t["default"] = r
	}
	
	
	, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "shouldComponentUpdate",
					value: function(e, t) {
						return !1
					}
				}, {
					key: "emitContactUsModalActivate",
					value: function(e) {
						App.events.emit("MODAL_ACTIVATE", {
							title: "Contact Us",
							type: "contact-us-modal"
						})
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: "footer flex-col"
						}, React.createElement("div", {
							className: "divider-colors"
						}, React.createElement("span", null), React.createElement("span", null), React.createElement("span", null), React.createElement("span", null)), React.createElement("div", {
							className: "row flex-row justify-center align-center"
						}, React.createElement("div", {
							className: "item flex-row align-center"
						}, "hanime.tv"), React.createElement("div", {
							className: "dash"
						}, "–"), React.createElement("div", {
							className: "item"
						}, React.createElement("span", {
							onClick: this.emitContactUsModalActivate,
							className: "transition-all link"
						}, "Contact Us")), React.createElement("div", {
							className: "dash"
						}, "–"), React.createElement("div", {
							className: "item"
						}, React.createElement("a", {
							href: "/search",
							className: "transition-all link"
						}, "Search Videos"))), React.createElement("div", {
							className: "row flex-row justify-center align-center "
						}, React.createElement("a", {
							className: "item flex-row align-center theporndude-color transition-all",
							href: "https://web.archive.org/web/20170201123401/http://theporndude.com/",
							title: "The Porn Dude: Discover Top Porn Sites!"
						}, React.createElement("div", {
							className: "flex-col align-center"
						}, React.createElement("div", {
							className: "image-holder"
						}, React.createElement("img", {
							className: "b-lazy b-lazy-pop-in iconize iconize-theporndude",
							src: App.transparent,
							"data-src": "https://web.archive.org/web/20170201123401/https://static1.hanime.tv/images/the_porn_dude_logo_grayscale.png",
							alt: "The Porn Dude: Discover Top Porn Sites!"
						}), React.createElement("img", {
							className: "b-lazy b-lazy-pop-in iconize iconize-theporndude active",
							src: App.transparent,
							"data-src": "https://web.archive.org/web/20170201123401/https://static2.hanime.tv/images/the_porn_dude_logo.png",
							alt: "The Porn Dude: Discover Top Porn Sites!"
						})), React.createElement("span", {
							className: "icon-text"
						}, "Discover"))), React.createElement("a", {
							className: "item flex-row align-center nutaku-color transition-all",
							href: "https://web.archive.org/web/20170201123401/https://ads2.contentabc.com/ads?spot_id=1618418",
							title: "Nutaku.com - Top Free Games Online"
						}, React.createElement("div", {
							className: "flex-col align-center"
						}, React.createElement("div", {
							className: "image-holder"
						}, React.createElement("img", {
							className: "b-lazy b-lazy-pop-in iconize iconize-nutaku passive",
							src: App.transparent,
							"data-src": "https://web.archive.org/web/20170201123401/https://static4.hanime.tv/images/nutaku_logo_grayscale.png",
							alt: "Nutaku.com - Top Free Games Online"
						}), React.createElement("img", {
							className: "b-lazy b-lazy-pop-in iconize iconize-nutaku active",
							src: App.transparent,
							"data-src": "https://web.archive.org/web/20170201123401/https://static3.hanime.tv/images/nutaku_logo.png",
							alt: "Nutaku.com - Top Free Games Online"
						})), React.createElement("span", {
							className: "icon-text"
						}, "Games")))))
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		
		
	


















	
		
		
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						ads: {
							landing_adhesion_1: {
								tablet: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "728",
											scrolling: "no",
											height: "90",
											frameBorder: "0",
											src: "",
											allowTransparency: "false",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "728px",
										height: "104px"
									}
								},
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "900",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "900px",
										height: "264px"
									}
								}
							},
							landing_adhesion_2: {
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "900",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "900px",
										height: "264px"
									}
								}
							},
							landing_adhesion_3: {
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "900",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "900px",
										height: "264px"
									}
								}
							},
							landing_footer_a: {
								tablet: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "300",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "",
											allowTransparency: "false",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "300px",
										height: "264px"
									}
								},
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "950",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0",
											name: "spot_id_1211926"
										})
									},
									style: {
										width: "950px",
										height: "264px"
									}
								}
							},
							landing_footer_b: {
								tablet: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "950",
											scrolling: "no",
											height: "275",
											frameBorder: "0",
											src: "",
											allowTransparency: "false",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "950px",
										height: "289px"
									}
								},
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "950",
											scrolling: "no",
											height: "275",
											frameBorder: "0",
											src: "",
											allowTransparency: "false",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "950px",
										height: "289px"
									}
								}
							},
							search_banner_top: {},
							search_banner_1: {
								tablet: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "300",
											scrolling: "no",
											height: "60",
											frameBorder: "0",
											src: "",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "300px",
										height: "74px"
									}
								},
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "475",
											scrolling: "no",
											height: "125",
											frameBorder: "0",
											src: "//web.archive.org/web/20170201123401/https://spot-01.atas.io/5817680573b4db24458b45f9?params[cv1]={publisher_ID}&params[cv2]={xuid}",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "475px",
										height: "139px"
									}
								}
							},
							video_ntv_a: {
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "300",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "https://web.archive.org/web/20170201123401/https://ads2.contentabc.com/ads?spot_id=1119644&rand=916582234",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0",
											name: "spot_id_1119644"
										})
									},
									style: {
										width: "300px",
										height: "264px"
									}
								}
							},
							video_ntv_b: {
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "300",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "https://web.archive.org/web/20170201123401/https://s3.atas.io/578ea75ac6dd2cd5518b4568?params[var]={publisher_ID}",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "300px",
										height: "264px"
									}
								}
							},
							video_ntv_c: {
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "160",
											scrolling: "no",
											height: "600",
											frameBorder: "0",
											src: "https://web.archive.org/web/20170201123401/https://ads2.contentabc.com/ads?spot_id=1498746&rand=988431748",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0",
											name: "spot_id_1498746"
										})
									},
									style: {
										width: "160px",
										height: "614px"
									}
								}
							},
							video_banner_after_content_banner_1: {
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "950",
											scrolling: "no",
											height: "250",
											frameBorder: "0",
											src: "https://web.archive.org/web/20170201123401/https://ads2.contentabc.com/ads?spot_id=1211932&rand=1967637170",
											allowTransparency: "true",
											marginHeight: "0",
											marginWidth: "0",
											name: "spot_id_1211932"
										})
									},
									style: {
										width: "950px",
										height: "264px"
									}
								}
							},
							video_banner_after_content_banner_2: {
								tablet: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "950",
											scrolling: "no",
											height: "275",
											frameBorder: "0",
											src: "https://web.archive.org/web/20170201123401/https://htvanime.com/tablet.html",
											allowTransparency: "false",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "950px",
										height: "289px"
									}
								},
								desktop: {
									html: function(e) {
										return React.createElement("iframe", {
											className: e,
											width: "950",
											scrolling: "no",
											height: "275",
											frameBorder: "0",
											src: "https://web.archive.org/web/20170201123401/https://htvanime.com/widget.html",
											allowTransparency: "false",
											marginHeight: "0",
											marginWidth: "0"
										})
									},
									style: {
										width: "950px",
										height: "289px"
									}
								}
							}
						},
						adspot: null
					}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.setState({
							adspot: this.state.ads[this.props.id]
						})
					}
				}, {
					key: "componentWillUnmount",
					value: function() {}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						App.events.addListener("PAGE_INITIALIZED", function() {
							e.forceUpdate()
						})
					}
				}, {
					key: "shouldComponentUpdate",
					value: function(e, t) {
						return e.is_ads_enabled != this.props.is_ads_enabled ? !0 : e.viewport_width != this.props.viewport_width ? !0 : e.scroll_top != this.props.scroll_top
					}
				}, {
					key: "getViewMode",
					value: function() {
						if (this.props.view_mode_override) return this.props.view_mode_override;
						var e = this.props.viewport_width,
							t = null;
						return t = 480 >= e ? "mobile" : 950 >= e ? "tablet" : "desktop"
					}
				}, 
				{
					key: "render",
					value: function() {
						return this.props.is_ads_enabled && this.state.adspot && this.state.adspot[this.getViewMode()] ? React.createElement("div", {
							className: classNames("golden-saucer", this.props.className),
							style: this.state.adspot[this.getViewMode()].style
						}, this.props.is_sponsor_text_disabled ? null : React.createElement("div", {
							className: "sponsor"
						}, "Sponsor"), this.props.is_sponsor_text_disabled ? null : React.createElement("div", {
							className: "msg"
						}, React.createElement("span", null, "We are supported primarily by advertisements. Please whitelist us so we can continue to build new features. You'll thank us later. :)")), this.state.adspot[this.getViewMode()].html(this.props.ad_class_names)) : null
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						family_id: e.model + "::" + e.associated_object_model + "::" + e.associated_object.id,
						is_showing_preempt: !1,
						preempt_favorites_count: null,
						preempt_favorite: null
					}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this,
							t = this.props.model + "::" + this.props.associated_object_model + "::" + this.props.associated_object.id;
						App.events.addListener("toggle-favorite-preempt|" + t, function(t) {
							e.setState({
								is_showing_preempt: !0,
								preempt_favorite: t.preempt_favorite,
								preempt_favorites_count: t.preempt_favorites_count
							})
						}), App.events.addListener("toggle-favorite-preempt-finished-ajax|" + t, function(t) {
							e.setState({
								is_showing_preempt: !1,
								preempt_favorite: null,
								preempt_favorites_count: e.props.favorites_count
							})
						})
					}
				}, {
					key: "heartIcon",
					value: function() {
						return this.state.is_showing_preempt ? this.state.preempt_favorite ? "fa-heart" : "fa-heart-o" : this.props.favorite ? "fa-heart" : "fa-heart-o"
					}
				}, {
					key: "toggleFavorite",
					value: function(e) {
						if (e.preventDefault(), e.stopPropagation(), !this.props.current_user) return void App.events.emit("toggle-favorite-not-logged-in-prompt");
						if (!this.state.is_showing_preempt) {
							if (this.props.favorite) App.events.emit("toggle-favorite-preempt|" + this.state.family_id, {
								preempt_favorite: null,
								preempt_favorites_count: this.props.favorites_count - 1
							}), $.ajax({
								type: "DELETE",
								url: this.props.rest_endpoint + "/" + this.props.favorite.id,
								success: this.preemptDestroyResolved,
								error: this.preemptDestroyFailed
							});
							else {
								App.events.emit("toggle-favorite-preempt|" + this.state.family_id, {
									preempt_favorite: {
										is_placeholder: !0
									},
									preempt_favorites_count: this.props.favorites_count + 1
								});
								var t = {};
								t[this.props.model] = {}, t[this.props.model][this.props.associated_object_model + "_id"] = this.props.associated_object.id, $.ajax({
									type: "POST",
									url: this.props.rest_endpoint,
									data: t,
									success: this.preemptCreateResolved,
									error: this.preemptCreateFailed
								})
							}
							return !1
						}
					}
				}, {
					key: "preemptCreateResolved",
					value: function(e) {
						App.events.emit("favorite-created", {
							favorite: e
						}), App.events.emit("toggle-favorite-preempt-finished-ajax|" + this.state.family_id, {})
					}
				}, {
					key: "preemptCreateFailed",
					value: function(e) {
						App.events.emit("toggle-favorite-preempt-finished-ajax|" + this.state.family_id, {})
					}
				}, {
					key: "preemptDestroyResolved",
					value: function(e) {
						App.events.emit("favorite-destroyed", {
							associated_object_id: this.props.associated_object.id
						}), App.events.emit("toggle-favorite-preempt-finished-ajax|" + this.state.family_id, {})
					}
				}, {
					key: "preemptDestroyFailed",
					value: function(e) {
						App.events.emit("toggle-favorite-preempt-finished-ajax|" + this.state.family_id, {})
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: classNames(this.props.className, "favorite", {}),
							onMouseDown: this.doNothing,
							onTouchStart: this.toggleFavorite,
							onClick: this.toggleFavorite,
							onTouchEnd: this.doNothing
						}, this.props.is_favorites_count_visible ? React.createElement("span", {
							className: "favorites-count grows-on-hover"
						}, this.state.is_showing_preempt ? this.state.preempt_favorites_count : this.props.favorites_count) : null, React.createElement("em", {
							className: classNames("fa grows-on-hover", this.heartIcon())
						}), this.props.children)
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
				return typeof e
			} : function(e) {
				return e && "function" == typeof Symbol && e.constructor === Symbol ? "symbol" : typeof e
			},
			r = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			o = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						width: 0,
						height: 0,
						focused_index: null,
						num_primary_slides: 0,
						smallest_left: 0,
						current_left_position: 0,
						sliding_container_styles: {},
						is_moving_slider: !1,
						body_has_animation_event_attached: !1,
						touch_start_focused_index: null,
						goto_url: null
					}, i
				}
				return s(t, e), r(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.updateStateOnWindowResize(), this.setState({
							is_touch_enabled: Modernizr.touchevents
						}, function() {})
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						window.addEventListener("resize", _.debounce(this.updateStateOnWindowResize, 300, {
							leading: !0,
							trailing: !0
						}))
					}
				}, {
					key: "shouldComponentUpdate",
					value: function(e, t) {
						return t.focused_index != this.state.focused_index ? !0 : t.current_left_position != this.state.current_left_position ? !0 : t.is_touch_enabled != this.state.is_touch_enabled ? !0 : e.slider_items != this.props.slider_items
					}
				}, {
					key: "updateStateOnWindowResize",
					value: function() {
						var e = window.innerWidth,
							t = window.innerHeight,
							a = 2;
						a = this.props.num_primary_slides_fn ? this.props.num_primary_slides_fn(e) : 500 > e ? 2 : 800 > e ? 3 : 1100 > e ? 4 : 1400 > e ? 5 : 6;
						var n = 92 / a,
							s = n * this.props.slider_items.length,
							i = -1 * s,
							r = this.state.current_left_position;
						i > r && (r = i);
						var o = {};
						this.state.touchevents ? (r = 0, o = {}) : o = {
							WebkitTransform: "translate3d(" + (r + 4) + "%, 0px, 0px)",
							transform: "translate3d(" + (r + 4) + "%, 0px, 0px)"
						};
						var c = {
							width: e,
							height: t,
							num_primary_slides: a,
							smallest_left: i,
							current_left_position: r,
							sliding_container_styles: o
						};
						this.setState(c)
					}
				}, {
					key: "prevSlides",
					value: function() {
						var e = 4;
						if (this.state.current_left_position + 92 > 0) {
							var t = 0;
							this.setState({
								current_left_position: t,
								sliding_container_styles: {
									WebkitTransform: "translate3d(" + (t + e) + "%, 0px, 0px)",
									transform: "translate3d(" + (t + e) + "%, 0px, 0px)"
								}
							})
						} else {
							var a = this.state.current_left_position + 92;
							this.setState({
								current_left_position: a,
								sliding_container_styles: {
									WebkitTransform: "translate3d(" + (a + e) + "%, 0px, 0px)",
									transform: "translate3d(" + (a + e) + "%, 0px, 0px)"
								}
							})
						}
						bLazy && "object" == ("undefined" == typeof bLazy ? "undefined" : i(bLazy)) && bLazy.revalidate && "function" == typeof bLazy.revalidate && setTimeout(function() {
							bLazy.revalidate()
						}, 400)
					}
				}, {
					key: "nextSlides",
					value: function() {
						var e = 4;
						if (this.state.current_left_position - 92 <= this.state.smallest_left + 92) {
							var t = this.state.smallest_left + 92;
							this.setState({
								current_left_position: t,
								sliding_container_styles: {
									transform: "translate3d(" + (t + e) + "%, 0px, 0px)",
									WebkitTransform: "translate3d(" + (t + e) + "%, 0px, 0px)"
								}
							})
						} else {
							var a = this.state.current_left_position - 92;
							this.setState({
								current_left_position: a,
								sliding_container_styles: {
									transform: "translate3d(" + (a + e) + "%, 0px, 0px)",
									WebkitTransform: "translate3d(" + (a + e) + "%, 0px, 0px)"
								}
							})
						}
						bLazy && "object" == ("undefined" == typeof bLazy ? "undefined" : i(bLazy)) && bLazy.revalidate && "function" == typeof bLazy.revalidate && setTimeout(function() {
							bLazy.revalidate()
						}, 400)
					}
				}, {
					key: "onTouchMoveSlidingContainer",
					value: function(e) {
						return null == this.state.focused_index && this.state.is_moving_slider === !0 ? !0 : (this.setState({
							focused_index: null,
							is_moving_slider: !0
						}), !0)
					}
				}, {
					key: "onTouchStartOnItem",
					value: function(e, t) {
						this.setState({
							touch_start_focused_index: t
						})
					}
				}, {
					key: "onTouchMoveOnItem",
					value: function(e, t) {
						this.setState({
							touch_start_focused_index: null
						})
					}
				}, {
					key: "onTouchEndOnItem",
					value: function(e, t) {
						this.state.touch_start_focused_index == t ? this.setState({
							focused_index: t,
							touch_start_focused_index: null
						}) : this.setState({
							touch_start_focused_index: null
						})
					}
				}, {
					key: "onMouseEnterItem",
					value: function(e, t) {
						e.preventDefault(), e.stopPropagation(), this.setState({
							focused_index: t
						})
					}
				}, {
					key: "onMouseLeaveItem",
					value: function(e, t) {
						e.preventDefault(), e.stopPropagation(), this.setState({
							focused_index: null
						})
					}
				}, {
					key: "activateSliderItem",
					value: function(e, t) {
						var a = this;
						return e.preventDefault(), e.stopPropagation(), $("body").removeClass("fade-zoom-in"), this.setState({
							goto_url: t
						}, function() {
							a.state.body_has_animation_event_attached || (App.cssAnimationEvent(document.getElementById("body"), "AnimationStart", function() {
								window.location.href = a.state.goto_url
							}), a.setState({
								body_has_animation_event_attached: !0
							})), setTimeout(function() {
								$("body").addClass("fade-zoom-in")
							}, 1)
						}), !1
					}
				}, {
					key: "itemAdjustmentCssClass",
					value: function(e) {
						var t = this.state.focused_index;
						return null == t ? "" : e == t ? t % this.state.num_primary_slides == 0 ? "focused-grow-right" : t % this.state.num_primary_slides == this.state.num_primary_slides - 1 ? "focused-grow-left" : "focused" : t > e && e >= t - 6 ? t % this.state.num_primary_slides == 0 ? void 0 : t % this.state.num_primary_slides == this.state.num_primary_slides - 1 ? "move-left-far" : "move-left" : e > t && t + 6 >= e ? t % this.state.num_primary_slides == 0 ? "move-right-far" : t % this.state.num_primary_slides == this.state.num_primary_slides - 1 ? void 0 : "move-right" : ""
					}
				}, {
					key: "htvSliderSimpleScroll",
					value: function() {
						var e = this,
							t = document.querySelectorAll(".htv-slider-simple .htv-lazy");
						_.each(t, function(t) {
							var a = t.getBoundingClientRect();
							return a.left > e.state.viewport_width ? !1 : (t.src = t.attributes["data-src"].value, void(t.className = t.className.replace(/htv\-lazy/, "htv-lazy-loaded")))
						})
					}
				}, {
					key: "renderX",
					value: function() {
						return this.state.is_touch_enabled ? this.renderSimple() : this.renderAdvanced()
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: "htv-slider"
						}, React.createElement("div", {
							className: "items-container"
						}, React.createElement("div", {
							className: classNames("handle handle-left", {
								disabled: this.state.current_left_position >= 0
							}),
							onMouseDown: this.prevSlides,
							onTouchStart: this.prevSlides
						}, React.createElement("em", {
							className: "fa fa-2x fa-angle-left"
						})), React.createElement("div", {
							className: "sliding-container",
							style: this.state.sliding_container_styles,
							onTouchMove: this.onTouchMoveSlidingContainer
						}, _.map(this.props.slider_items, function(t, a) {
							return e.props.disable_slider_item_id && t.id && t.id == e.props.disable_slider_item_id ? React.createElement("div", {
								className: classNames("item", e.itemAdjustmentCssClass(a)),
								key: a
							}, e.renderChildren(t, a, !0)) : React.createElement("div", {
								className: classNames("item", e.itemAdjustmentCssClass(a)),
								key: a,
								onMouseEnter: function(t) {
									e.onMouseEnterItem(t, a)
								},
								onMouseLeave: function(t) {
									e.onMouseLeaveItem(t, a)
								},
								onTouchStart: function(t) {
									e.onTouchStartOnItem(t, a)
								},
								onTouchMove: function(t) {
									e.onTouchMoveOnItem(t, a)
								},
								onTouchEnd: function(t) {
									e.onTouchEndOnItem(t, a)
								}
							}, e.renderChildren(t, a))
						})), React.createElement("div", {
							className: classNames("handle handle-right", {
								disabled: this.state.current_left_position <= this.state.smallest_left + 92
							}),
							onMouseDown: this.nextSlides,
							onTouchStart: this.nextSlides
						}, React.createElement("em", {
							className: "fa fa-2x fa-angle-right"
						}))))
					}
				}, {
					key: "renderChildren",
					value: function(e, t, a) {
						var n = this;
						return React.Children.map(this.props.children, function(s) {
							return React.cloneElement(s, {
								data: e,
								on_activate_function: n.activateSliderItem,
								is_focused: t == n.state.focused_index,
								is_disabled: a
							})
						})
					}
				}]), t
			}(React.Component);
		t["default"] = o
	}, function(e, t) {
		function a() {
			l = !1, r.length ? c = r.concat(c) : u = -1, c.length && n()
		}

		function n() {
			if (!l) {
				var e = setTimeout(a);
				l = !0;
				for (var t = c.length; t;) {
					for (r = c, c = []; ++u < t;) r && r[u].run();
					u = -1, t = c.length
				}
				r = null, l = !1, clearTimeout(e)
			}
		}

		function s(e, t) {
			this.fun = e, this.array = t
		}

		function i() {}
		var r, o = e.exports = {},
			c = [],
			l = !1,
			u = -1;
		o.nextTick = function(e) {
			var t = new Array(arguments.length - 1);
			if (arguments.length > 1)
				for (var a = 1; a < arguments.length; a++) t[a - 1] = arguments[a];
			c.push(new s(e, t)), 1 !== c.length || l || setTimeout(n, 0)
		}, s.prototype.run = function() {
			this.fun.apply(null, this.array)
		}, o.title = "browser", o.browser = !0, o.env = {}, o.argv = [], o.version = "", o.versions = {}, o.on = i, o.addListener = i, o.once = i, o.off = i, o.removeListener = i, o.removeAllListeners = i, o.emit = i, o.binding = function(e) {
			throw new Error("process.binding is not supported")
		}, o.cwd = function() {
			return "/"
		}, o.chdir = function(e) {
			throw new Error("process.chdir is not supported")
		}, o.umask = function() {
			return 0
		}
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(1),
			l = n(c),
			u = a(5),
			d = n(u),
			p = a(2),
			h = n(p),
			m = a(3),
			f = n(m),
			v = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), window.bLazy = new Blazy({})
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: "apps"
						}, React.createElement(l["default"], this.props), React.createElement("div", {
							className: "billboard b-lazy",
							"data-src": "/site-bg-1.jpg"
						}, React.createElement("div", {
							className: "bg-gradient"
						}), React.createElement("h1", null, "Enjoy our HD hentai collection anywhere, anytime"), React.createElement("p", {
							className: "subtext center"
						}, "Apps designed with users in mind.  Play videos on your", React.createElement("br", null), "desktop, tablet, phone, or offline on the go.")), React.createElement("div", {
							className: "download-row"
						}, React.createElement("a", {
							href: "https://web.archive.org/web/20170201123401/https://static1.hanime.tv/apks/htvh_v1_1_armv7.apk",
							className: "btn btn-primary download-btn",
							target: "_blank"
						}, React.createElement("span", {
							className: "fa fa-android fa-stacked"
						}), "  Download v1.1 now")), React.createElement("div", {
							className: "container points"
						}, React.createElement("div", {
							className: "point"
						}, React.createElement("div", {
							className: "point-image-container"
						}, React.createElement("img", {
							className: "any-device b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/macbook-v2.png",
							alt: "Our site is compatible with every modern browser",
							width: "100%"
						})), React.createElement("h2", null, "hanime", React.createElement("span", {
							className: "primary-color"
						}, "."), "tv", React.createElement("br", null), "on any device"), React.createElement("img", {
							className: "any-device-image b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/any-device.png"
						})), React.createElement("div", {
							className: "point"
						}, React.createElement("div", {
							className: "point-image-container"
						}, React.createElement("img", {
							className: "tablet b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/tablet.png",
							width: "100%"
						})), React.createElement("div", {
							className: ""
						}, React.createElement("h2", null, "HTV hentai", React.createElement("br", null), "mobile-optimized"), React.createElement("span", {
							className: "fa fa-android fa-4x"
						}))), React.createElement("div", {
							className: "point"
						}, React.createElement("div", {
							className: "point-image-container"
						}, React.createElement("img", {
							className: "native-video-player b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/native-video-player-v2.png",
							width: "100%"
						})), React.createElement("div", {
							className: ""
						}, React.createElement("h2", null, "Native video player", React.createElement("br", null), "experience"), React.createElement("div", {
							className: "point-info"
						}, "Smooth seek.", React.createElement("br", null), "Faster load.", React.createElement("br", null), "No dropped frames.")))), React.createElement("div", {
							className: "divider-colors"
						}, React.createElement("span", null), React.createElement("span", null), React.createElement("span", null), React.createElement("span", null)), React.createElement("div", {
							className: "download-n-instructions container",
							id: "download_n_instructions"
						}, React.createElement("div", {
							className: "instructions"
						}, React.createElement("h2", null, "How to install HTV hentai v1.1 on your Android device"), React.createElement("p", {
							className: "text"
						}, "HTV hentai is not available on the Google Play Store so we need to manually install using the following steps:"), React.createElement("ol", null, React.createElement("li", null, "Enable non-Google Play Store app installation on your Android device.", React.createElement("br", null), React.createElement("span", {
							className: "instruction-steps"
						}, React.createElement("strong", null, "Settings"), ">", React.createElement("strong", null, "General tab"), ">", React.createElement("strong", null, "Security tab"), "> Check ", React.createElement("strong", null, "Unknown Sources"), ">", React.createElement("strong", null, "Press OK")), React.createElement("div", {
							className: "instruction-images"
						}, React.createElement("a", {
							className: "s1",
							href: "/images/s1-settings.jpg",
							target: "_blank"
						}, React.createElement("img", {
							className: "b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/s1-settings.jpg"
						})), React.createElement("a", {
							className: "s2",
							href: "/images/s2-general.jpg",
							target: "_blank"
						}, React.createElement("img", {
							className: "b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/s2-general.jpg"
						})), React.createElement("a", {
							className: "s3",
							href: "/images/s3-security.jpg",
							target: "_blank"
						}, React.createElement("img", {
							className: "b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/s3-security.jpg"
						})), React.createElement("a", {
							className: "s4",
							href: "/images/s4-unknown.jpg",
							target: "_blank"
						}, React.createElement("img", {
							className: "b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/s4-unknown.jpg"
						})), React.createElement("a", {
							className: "s5",
							href: "/images/s5-clickok.jpg",
							target: "_blank"
						}, React.createElement("img", {
							className: "b-lazy b-lazy-pop-in",
							src: App.transparent,
							"data-src": "/images/s5-clickok.jpg"
						}))), React.createElement("div", {
							className: "youtube"
						}, "Still having trouble?  Try the ", React.createElement("a", {
							className: "bold",
							href: "https://web.archive.org/web/20170201123401/https://www.youtube.com/watch?v=g5n71QXLLgw",
							target: "_blank"
						}, "Youtube video instructions"), ".")), React.createElement("li", null, "Download the application on your device:", React.createElement("div", {
							className: "download-row"
						}, React.createElement("a", {
							className: "btn btn-primary download-btn",
							href: "https://web.archive.org/web/20170201123401/https://static1.hanime.tv/apks/htvh_v1_1_armv7.apk",
							target: "_blank"
						}, React.createElement("span", {
							className: "fa fa-android fa-stacked"
						}), "  Download v1.1 now")), React.createElement("div", {
							className: "alt-download"
						}, "Can't install the file?  Try installing this  ", React.createElement("a", {
							className: "bold",
							href: "https://web.archive.org/web/20170201123401/https://static1.hanime.tv/apks/htvh_v1_1_x86.apk",
							target: "_blank"
						}, "HTV hentai v1.1 x86 version"), ".")), React.createElement("li", null, "Press on the downloaded APK file to install."), React.createElement("li", null, "Open the HTV hentai v1.1 application and enjoy.")))), React.createElement("div", {
							className: "divider-colors"
						}, React.createElement("span", null), React.createElement("span", null), React.createElement("span", null), React.createElement("span", null)), React.createElement("div", {
							className: "troubleshooting container"
						}, React.createElement("h2", null, "Troubleshooting / Frequently Asked Questions"), React.createElement("ul", null, React.createElement("li", null, React.createElement("p", {
							className: "question"
						}, "Q: I can't see videos!  The app doesn't work!"), React.createElement("p", null, "A: Your Android device lacks a built-in video player.  To fix this problem, go to the Google Play Store and download then install either BSPlayer or MXPlayer - then try ", React.createElement("span", {
							className: "bold"
						}, "HTV hentai"), " again.")), React.createElement("li", null, React.createElement("p", {
							className: "question"
						}, "Q: Why does the app seem ", React.createElement("em", null, "slow"), "?"), React.createElement("p", null, "A: Android hardware and software range greatly in performance.  We are working on optimizing the app for speed, coming in version 2.0.")), React.createElement("li", null, React.createElement("p", {
							className: "question"
						}, "Q: Will there ever be an iOS app?"), React.createElement("p", null, "A: We have a solution in the works for getting you guys the iOS app.  It may require some additional effort.")), React.createElement("li", null, React.createElement("p", {
							className: "question"
						}, "Q: Can you guys add login/logout so we can view our favorite videos?"), React.createElement("p", null, "A: Yes, this feature is important and is definitely on the roadmap for v2.0.")), React.createElement("li", null, React.createElement("p", {
							className: "question"
						}, "Q: When will v2.0 be released?"), React.createElement("p", null, 'A: "It will be done, when it\'s done. ®"  Seriously, the only project higher in priority is releasing ', React.createElement("span", {
							className: "bold"
						}, "HTV anime"), " on Android and iOS.")))), React.createElement(d["default"], null), React.createElement(h["default"], this.props), React.createElement(f["default"], this.props))
					}
				}]), t
			}(React.Component);
		t["default"] = v
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(1),
			l = n(c),
			u = a(8),
			d = (n(u), a(4)),
			p = (n(d), a(2)),
			h = n(p),
			m = a(3),
			f = n(m),
			v = a(7),
			g = n(v),
			y = a(5),
			b = n(y),
			E = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						hentai_videos: n.props.hentai_videos,
						hentai_video_favorites: n.props.hentai_video_favorites,
						is_reorganizing: !1
					}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), window.bLazy = new Blazy({})
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						App.events.addListener("favorite-created", this.favoriteCreated), App.events.addListener("favorite-destroyed", this.favoriteDestroyed)
					}
				}, {
					key: "favoriteDestroyed",
					value: function(e) {
						var t = _.map(this.state.hentai_video_favorites, _.clone),
							a = _.filter(t, {
								hentai_video_id: e.associated_object_id
							});
						a.length > 0 && _.remove(t, a[0]);
						var n = _.map(this.state.hentai_videos, _.clone),
							s = _.filter(n, {
								id: e.associated_object_id
							});
						s.length > 0 && s[0].favorites_count--, this.setState({
							hentai_videos: n,
							hentai_video_favorites: t
						})
					}
				}, {
					key: "favoriteCreated",
					value: function(e) {
						var t = _.find(this.state.hentai_video_favorites, e.favorite);
						if ("undefined" == typeof t) {
							var a = _.map(this.state.hentai_video_favorites, _.clone);
							a.push(e.favorite);
							var n = _.map(this.state.hentai_videos, _.clone),
								s = _.filter(n, {
									id: e.favorite.hentai_video_id
								});
							s.length > 0 && s[0].favorites_count++, this.setState({
								hentai_videos: n,
								hentai_video_favorites: a
							})
						}
					}
				}, {
					key: "getHentaiVideoFavorite",
					value: function(e) {
						var t = this.props.hentai_video_favorites;
						this.state && (t = this.state.hentai_video_favorites);
						var a = _.filter(t, {
							hentai_video_id: e
						});
						return a.length > 0 ? a[0] : null
					}
				}, {
					key: "getFavoriteComponent",
					value: function(e) {
						return React.createElement(g["default"], {
							className: "favorites",
							favorite: this.getHentaiVideoFavorite(e.id),
							favorites_count: e.favorites_count,
							is_favorites_count_visible: !0,
							rest_endpoint: "/api/v1/hentai_video_favorites",
							model: "hentai_video_favorite",
							associated_object_model: "hentai_video",
							associated_object: e,
							current_user: this.props.current_user
						})
					}
				}, {
					key: "getUrl",
					value: function(e) {
						return "/hentai-videos/" + e.slug + "?r=/favorites"
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: "my-favorites"
						}, React.createElement(l["default"], this.props), React.createElement("div", {
							className: "content clearfix"
						}, _.map(this.state.hentai_video_favorites, function(t, a) {
							var n = _.find(e.state.hentai_videos, {
								id: t.hentai_video_id
							});
							return React.createElement("a", {
								className: "my-favorite",
								key: a,
								href: e.getUrl(n)
							}, React.createElement("div", {
								className: "icon-container"
							}, React.createElement("div", {
								className: "outer"
							}, React.createElement("div", {
								className: "inner"
							}, React.createElement("div", {
								className: "icon b-lazy",
								"data-src": n.cover_url
							})))), React.createElement("div", {
								className: "title"
							}, n.name))
						})), React.createElement(b["default"], null), React.createElement(h["default"], this.props), React.createElement(f["default"], this.props))
					}
				}]), t
			}(React.Component);
		t["default"] = E
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(1),
			l = n(c),
			u = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						form: {
							email: "",
							user_agent: "",
							screen_width: "",
							screen_height: "",
							operating_system: ""
						},
						is_submitting: !1,
						is_done: !1,
						status_text_class: "danger",
						status_text: ""
					}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.state.form.user_agent = navigator.userAgent, this.state.form.screen_width = screen.width, this.state.form.screen_height = screen.height, this.state.form.operating_system = jscd.os + " " + jscd.osVersion, $("#email").focus()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "sendPasswordReset",
					value: function() {
						var e = this;
						this.isSendPasswordResetButtonEnabled() && (this.setState({
							is_submitting: !0
						}), $.post("/api/v1/user_passwords", {
							user: this.state.form
						}).done(function(t) {
							e.setState({
								is_done: !0,
								status_text_class: "success",
								status_text: "We have sent a password reset email to your email account.  Please check your inbox for next steps."
							})
						}).fail(function(t) {
							var a = t.statusText;
							t.responseJSON && (a = t.responseJSON.errors), e.setState({
								status_text_class: "danger",
								status_text: a,
								is_submitting: !1
							})
						}).always(function() {}))
					}
				}, {
					key: "updateForm",
					value: function(e, t) {
						var a = this.state.form;
						a[t] = e.target.value, this.setState({
							form: a
						})
					}
				}, {
					key: "isSendPasswordResetButtonEnabled",
					value: function() {
						return App.isValidEmail(this.state.form.email) ? !this.state.is_submitting : !1
					}
				}, {
					key: "handleNext",
					value: function(e, t, a) {
						13 == e.which && ("forgot-password" == a ? this.sendPasswordReset() : $(t).focus())
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: "forgot-password has-bg"
						}, React.createElement(l["default"], this.props), React.createElement("div", {
							className: "panel"
						}, React.createElement("div", {
							className: "panel-section"
						}, React.createElement("div", {
							className: "ribbon ribbon-small ribbon-orange"
						}, React.createElement("div", {
							className: "banner"
						}, React.createElement("h2", {
							className: "text"
						}, React.createElement("em", {
							className: "fa fa-lock"
						}), "  SSL"))), React.createElement("a", {
							href: "/"
						}, React.createElement("img", {
							src: "logo-100.png",
							className: "logo",
							alt: "Free Anime Hentai HD Streams for Mobile"
						})), React.createElement("h1", null, "Forgot Password"), React.createElement("input", {
							className: "input-responsive",
							id: "email",
							type: "email",
							placeholder: "Email Address",
							onChange: function(t) {
								e.updateForm(t, "email")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "", "forgot-password")
							}
						}), this.state.status_text ? React.createElement("div", {
							className: classNames("status-text", this.state.status_text_class)
						}, this.state.status_text) : null, React.createElement("div", {
							className: "row"
						}, React.createElement("div", {
							className: "col-1"
						}, this.state.is_done ? null : React.createElement("button", {
							className: classNames("button button-primary button-sm button-responsive", {
								disabled: !this.isSendPasswordResetButtonEnabled()
							}),
							onClick: this.sendPasswordReset
						}, this.state.is_submitting ? React.createElement("span", null, React.createElement("em", {
							className: "fa fa-spinner fa-spin"
						})) : React.createElement("span", null, "Send Password Reset Email"))))), React.createElement("div", {
							className: "panel-section panel-section-dark"
						}, React.createElement("div", {
							className: "panel-text"
						}, "New to ", this.props.env.domain_name, "?"), React.createElement("a", {
							href: "/create-account",
							className: "button button-sm button-responsive"
						}, "Create a Free Account"))))
					}
				}]), t
			}(React.Component);
		t["default"] = u
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(1),
			l = n(c),
			u = a(8),
			d = n(u),
			p = a(4),
			h = n(p),
			m = a(2),
			f = n(m),
			v = a(3),
			g = n(v),
			y = a(7),
			b = n(y),
			E = a(5),
			w = n(E),
			R = a(6),
			N = n(R),
			k = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						max_scroll_top: 0,
						viewport_width: 0,
						viewport_height: 0,
						hentai_videos: e.hentai_videos,
						hentai_video_favorites: e.hentai_video_favorites,
						is_subsection_3_triggered: !1,
						is_subsection_4_triggered: !1,
						is_page_initialized: !1
					}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.updateViewportDimensions(), window.bLazy = new Blazy({
							container: ".items-container"
						}), this.setState({
							is_page_initialized: !0
						}, function() {
							App.events.emit("PAGE_INITIALIZED")
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						window.addEventListener("resize", _.debounce(this.updateViewportDimensions, 500, {
							trailing: !0
						})), window.addEventListener("scroll", _.debounce(this.updateScrollTop, 150, {
							leading: !0,
							trailing: !0
						})), App.events.addListener("favorite-created", this.favoriteCreated), App.events.addListener("favorite-destroyed", this.favoriteDestroyed), App.events.addListener("toggle-favorite-not-logged-in-prompt", function() {
							App.events.emit("MODAL_ACTIVATE", {
								title: "Login Required",
								type: "login-required-modal",
								body: "Adding this hentai episode to your favorites list requires logging in!"
							})
						})
					}
				}, {
					key: "shouldComponentUpdate",
					value: function(e, t) {
						return t.hentai_videos != this.state.hentai_videos ? !0 : t.hentai_video_favorites != this.state.hentai_video_favorites ? !0 : t.viewport_width != this.state.viewport_width ? !0 : t.max_scroll_top != this.state.max_scroll_top ? !0 : t.is_page_initialized != this.state.is_page_initialized
					}
				}, {
					key: "updateScrollTop",
					value: function() {
						var e = this,
							t = $(window).scrollTop(),
							a = Math.max(t, this.state.max_scroll_top);
						this.setState({
							max_scroll_top: a
						}, function() {
							100 > a || (300 > a && !e.state.is_subsection_3_triggered ? (window.bLazy = new Blazy({
								container: ".items-container"
							}), e.setState({
								is_subsection_3_triggered: !0
							})) : a >= 300 && !e.state.is_subsection_4_triggered && (window.bLazy = new Blazy({
								container: ".items-container"
							}), e.setState({
								is_subsection_4_triggered: !0
							})))
						})
					}
				}, {
					key: "updateViewportDimensions",
					value: function() {
						this.setState({
							viewport_width: $(window).width(),
							viewport_height: $(window).height()
						})
					}
				}, {
					key: "favoriteDestroyed",
					value: function(e) {
						var t = _.map(this.state.hentai_video_favorites, _.clone),
							a = _.filter(t, {
								hentai_video_id: e.associated_object_id
							});
						a.length > 0 && _.remove(t, a[0]);
						var n = _.map(this.state.hentai_videos, _.clone),
							s = _.filter(n, {
								id: e.associated_object_id
							});
						s.length > 0 && s[0].favorites_count--, this.setState({
							hentai_videos: n,
							hentai_video_favorites: t
						})
					}
				}, {
					key: "favoriteCreated",
					value: function(e) {
						var t = _.find(this.state.hentai_video_favorites, e.favorite);
						if ("undefined" == typeof t) {
							var a = _.map(this.state.hentai_video_favorites, _.clone);
							a.push(e.favorite);
							var n = _.map(this.state.hentai_videos, _.clone),
								s = _.filter(n, {
									id: e.favorite.hentai_video_id
								});
							s.length > 0 && s[0].favorites_count++, this.setState({
								hentai_videos: n,
								hentai_video_favorites: a
							})
						}
					}
				}, {
					key: "getHentaiVideoFavorite",
					value: function(e) {
						var t = this.props.hentai_video_favorites;
						this.state && (t = this.state.hentai_video_favorites);
						var a = _.filter(t, {
							hentai_video_id: e
						});
						return a.length > 0 ? a[0] : null
					}
				}, {
					key: "getFavoriteComponent",
					value: function(e) {
						return React.createElement(b["default"], {
							className: "favorites",
							favorite: this.getHentaiVideoFavorite(e.id),
							favorites_count: e.favorites_count,
							is_favorites_count_visible: !0,
							rest_endpoint: "/api/v1/hentai_video_favorites",
							model: "hentai_video_favorite",
							associated_object_model: "hentai_video",
							associated_object: e,
							current_user: this.props.current_user
						})
					}
				}, {
					key: "getUrl",
					value: function(e) {
						return "/hentai-videos/" + e.slug
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: "landing"
						}, React.createElement(l["default"], this.props), React.createElement("div", {
							className: "content"
						}, React.createElement("div", {
							className: "billboard b-lazy",
							"data-src": "site-bg-1.jpg"
						}, React.createElement("div", {
							className: "bg-gradient"
						}), React.createElement("h1", null, "Watch Free HD Hentai & Anime Videos"), React.createElement("p", {
							className: "subtext center"
						}, "Enjoy your ", React.createElement("span", {
							className: "highlight"
						}, "unlimited"), "  hentai & anime collection.  We are the definitive source for the best curated 720p / 1080p HD hentai videos, viewable by mobile phone and tablet, for free.")), React.createElement("div", {
							className: "section"
						}, React.createElement("div", {
							className: "subsection subsection-1"
						}, React.createElement("h3", {
							className: "subsection-title"
						}, "Recent Uploads"), React.createElement(d["default"], {
							slider_items: _.map(this.props.recent_uploads_ids, function(t) {
								return _.find(e.state.hentai_videos, {
									id: t
								})
							})
						}, React.createElement(h["default"], {
							url_function: this.getUrl,
							addon: this.getFavoriteComponent
						}))), this.state.is_page_initialized ? React.createElement(N["default"], {
							className: "subsection z-spot",
							id: "landing_adhesion_1",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width
						}) : null, React.createElement("div", {
							className: "subsection"
						}, React.createElement("h3", {
							className: "subsection-title"
						}, "2017 New Releases"), React.createElement(d["default"], {
							slider_items: _.map(this.props.newest_ids, function(t) {
								return _.find(e.state.hentai_videos, {
									id: t
								})
							})
						}, React.createElement(h["default"], {
							url_function: this.getUrl,
							addon: this.getFavoriteComponent
						}))), this.state.is_page_initialized ? React.createElement(N["default"], {
							className: "subsection z-spot",
							id: "landing_adhesion_2",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width
						}) : null, this.state.max_scroll_top >= 100 ? React.createElement("div", {
							className: "subsection"
						}, React.createElement("h3", {
							className: "subsection-title"
						}, "Trending"), React.createElement(d["default"], {
							slider_items: _.map(this.props.trending_ids, function(t) {
								return _.find(e.state.hentai_videos, {
									id: t
								})
							})
						}, React.createElement(h["default"], {
							url_function: this.getUrl,
							addon: this.getFavoriteComponent
						}))) : null, this.state.is_page_initialized ? React.createElement(N["default"], {
							className: "subsection z-spot",
							id: "landing_adhesion_3",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width
						}) : null, this.state.max_scroll_top >= 300 ? React.createElement("div", {
							className: "subsection"
						}, React.createElement("h3", {
							className: "subsection-title"
						}, "Random"), React.createElement(d["default"], {
							slider_items: _.map(this.props.rand_ids, function(t) {
								return _.find(e.state.hentai_videos, {
									id: t
								})
							})
						}, React.createElement(h["default"], {
							url_function: this.getUrl,
							addon: this.getFavoriteComponent
						}))) : null), this.state.is_page_initialized ? React.createElement("div", {
							className: "section"
						}, React.createElement(N["default"], {
							className: "z-spot",
							id: "landing_footer_a",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width
						}), React.createElement(N["default"], {
							className: "z-spot",
							id: "landing_footer_b",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width,
							is_sponsor_text_disabled: !0
						})) : null), React.createElement(w["default"], null), React.createElement(f["default"], this.props), React.createElement(g["default"], this.props))
					}
				}]), t
			}(React.Component);
		t["default"] = k
	}, function(t, a, n) {
		"use strict";

		function s(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function i(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function r(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function o(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(a, "__esModule", {
			value: !0
		});
		var c = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			l = n(1),
			u = s(l),
			d = function(t) {
				function a(e, t) {
					i(this, a);
					var n = r(this, Object.getPrototypeOf(a).call(this, e, t)),
						s = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(s, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						form: {
							email: "",
							password: "",
							remember_me: "1",
							user_agent: "",
							screen_width: "",
							screen_height: "",
							operating_system: ""
						},
						is_submitting: !1,
						status_text: ""
					}, n
				}
				return o(a, t), c(a, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), $("#email").focus()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "logIn",
					value: function() {
						var t = this;
						this.isLogInButtonEnabled() && (this.setState({
							is_submitting: !0
						}), $.ajax({
							type: "POST",
							url: "/api/v2/sessions",
							data: {
								user: this.state.form
							},
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								t.setState({
									status_text: ""
								}), window.location = window.location.protocol + "//" + window.location.hostname + ":" + window.location.port
							},
							error: function(a) {
								t.setState({
									status_text: "Incorrect password or email.",
									is_submitting: !1
								}), e(a)
							}
						}))
					}
				}, {
					key: "updateForm",
					value: function(e, t) {
						var a = this.state.form;
						a[t] = e.target.value, this.setState({
							form: a
						})
					}
				}, {
					key: "isLogInButtonEnabled",
					value: function() {
						return "undefined" == typeof this.state.form.email || 0 == this.state.form.email.length ? !1 : this.state.form.password.length < 6 ? !1 : App.isValidEmail(this.state.form.email) ? !this.state.is_submitting : !1
					}
				}, {
					key: "handleNext",
					value: function(e, t, a) {
						13 == e.which && ("log-in" == a ? this.logIn() : $(t).focus())
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: "log-in has-bg"
						}, React.createElement(u["default"], this.props), React.createElement("div", {
							className: "panel"
						}, React.createElement("div", {
							className: "panel-section"
						}, React.createElement("div", {
							className: "ribbon ribbon-small ribbon-orange"
						}, React.createElement("div", {
							className: "banner"
						}, React.createElement("h2", {
							className: "text"
						}, React.createElement("em", {
							className: "fa fa-lock"
						}), "  SSL"))), React.createElement("a", {
							href: "/"
						}, React.createElement("img", {
							src: "logo-100.png",
							className: "logo",
							alt: "Free Anime Hentai HD Streams for Mobile"
						})), React.createElement("h1", null, "Login"), React.createElement("input", {
							className: "input-responsive",
							id: "email",
							type: "email",
							placeholder: "Email Address",
							onChange: function(t) {
								e.updateForm(t, "email")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "#password")
							}
						}), React.createElement("input", {
							className: "input-responsive",
							id: "password",
							type: "password",
							placeholder: "Password (6+ characters)",
							onChange: function(t) {
								e.updateForm(t, "password")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "", "log-in")
							}
						}), this.state.status_text ? React.createElement("div", {
							className: "status-text"
						}, this.state.status_text) : null, React.createElement("div", {
							className: "row"
						}, React.createElement("div", {
							className: "col-1"
						}, React.createElement("button", {
							className: classNames("button button-primary button-sm button-responsive", {
								disabled: !this.isLogInButtonEnabled()
							}),
							onClick: this.logIn
						}, this.state.is_submitting ? React.createElement("span", null, React.createElement("em", {
							className: "fa fa-spinner fa-spin"
						})) : React.createElement("span", null, "Login"))), React.createElement("div", {
							className: "col-2"
						}, React.createElement("a", {
							href: "/forgot-password",
							className: "button button-sm button-responsive"
						}, "Can't Log In?")))), React.createElement("div", {
							className: "panel-section panel-section-dark"
						}, React.createElement("div", {
							className: "panel-text"
						}, "New to ", this.props.env.domain_name, "?"), React.createElement("a", {
							href: "/create-account",
							className: "button button-sm button-responsive"
						}, "Create a Free Account"))))
					}
				}]), a
			}(React.Component);
		a["default"] = d
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(1),
			l = n(c),
			u = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						form: {
							password: "",
							password_confirmation: "",
							user_agent: "",
							screen_width: "",
							screen_height: "",
							operating_system: ""
						},
						is_token_valid: n.props.is_token_valid,
						is_submitting: !1,
						is_done: !1,
						status_text_class: "danger",
						status_text: ""
					}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.setState({
							form: {
								password: "",
								password_confirmation: "",
								user_agent: navigator.userAgent,
								screen_width: screen.width,
								screen_height: screen.height,
								operating_system: jscd.os + " " + jscd.osVersion
							}
						}), $("#password").focus()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "changePassword",
					value: function() {
						var e = this;
						this.isChangePasswordButtonEnabled() && (this.setState({
							is_submitting: !0
						}), $.ajax({
							type: "PUT",
							url: "/api/v1/user_passwords/" + this.props.reset_password_token,
							data: {
								user: this.state.form
							},
							success: function(t) {
								e.setState({
									is_done: !0,
									status_text_class: "success",
									status_text: "Password successfully updated!"
								})
							},
							error: function(t) {
								console.log("error:", t), e.setState({
									is_token_valid: !1
								})
							},
							complete: function(e, t) {}
						}))
					}
				}, {
					key: "updateForm",
					value: function(e, t) {
						var a = this.state.form;
						a[t] = e.target.value, this.setState({
							form: a
						})
					}
				}, {
					key: "isChangePasswordButtonEnabled",
					value: function() {
						return this.state.form.password.length < 6 ? !1 : 0 == this.state.form.password_confirmation.length ? !1 : this.state.form.password != this.state.form.password_confirmation ? !1 : !this.state.is_submitting
					}
				}, {
					key: "handleNext",
					value: function(e, t, a) {
						13 == e.which && ("change-password" == a ? this.changePassword() : $(t).focus())
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: "forgot-password has-bg"
						}, React.createElement(l["default"], this.props), React.createElement("div", {
							className: "panel"
						}, React.createElement("div", {
							className: "panel-section"
						}, React.createElement("div", {
							className: "ribbon ribbon-small ribbon-orange"
						}, React.createElement("div", {
							className: "banner"
						}, React.createElement("h2", {
							className: "text"
						}, React.createElement("em", {
							className: "fa fa-lock"
						}), "  SSL"))), this.state.is_token_valid ? this.renderValidTokenHtml() : this.renderInvalidTokenHtml())))
					}
				}, {
					key: "renderValidTokenHtml",
					value: function() {
						var e = this;
						return React.createElement("div", null, React.createElement("h1", null, "Change Password"), React.createElement("input", {
							className: "input-responsive",
							id: "password",
							type: "password",
							placeholder: "New Password (6+ characters)",
							onChange: function(t) {
								e.updateForm(t, "password")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "#password_confirmation")
							}
						}), React.createElement("input", {
							className: "input-responsive",
							id: "password_confirmation",
							type: "password",
							placeholder: "New Password Confirm",
							onChange: function(t) {
								e.updateForm(t, "password_confirmation")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "", "change-password")
							}
						}), this.state.status_text ? React.createElement("div", {
							className: classNames("status-text", this.state.status_text_class)
						}, this.state.status_text) : null, React.createElement("div", {
							className: "row"
						}, React.createElement("div", {
							className: "col-1"
						}, this.state.is_done ? React.createElement("a", {
							href: "/",
							className: "button button-primary button-sm button-responsive"
						}, "Go Back") : React.createElement("button", {
							className: classNames("button button-primary button-sm button-responsive", {
								disabled: !this.isChangePasswordButtonEnabled()
							}),
							onClick: this.changePassword
						}, this.state.is_submitting ? React.createElement("span", null, React.createElement("em", {
							className: "fa fa-spinner fa-spin"
						})) : React.createElement("span", null, "Change Password")))))
					}
				}, {
					key: "renderInvalidTokenHtml",
					value: function() {
						return React.createElement("div", null, React.createElement("h1", null, "Oops!"), React.createElement("div", {
							className: "error-message danger"
						}, "It looks like the link provided has expired. Please request a new reset password email from the  ", React.createElement("a", {
							href: "/forgot-password"
						}, "Forgot Password"), "  page."), React.createElement("br", null), React.createElement("br", null), React.createElement("a", {
							href: "/forgot-password",
							className: "button button-primary button-sm button-responsive"
						}, "Go to Forgot Password"))
					}
				}]), t
			}(React.Component);
		t["default"] = u
	}, function(t, a, n) {
		"use strict";

		function s(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function i(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function r(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function o(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(a, "__esModule", {
			value: !0
		});
		var c = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			u = n(1),
			d = s(u),
			p = n(2),
			h = s(p),
			m = n(3),
			f = s(m),
			v = n(27),
			g = s(v),
			y = n(25),
			b = s(y),
			E = n(6),
			w = s(E),
			R = n(31),
			N = s(R),
			k = function(t) {
				function a(e, t) {
					i(this, a);
					var n = r(this, Object.getPrototypeOf(a).call(this, e, t)),
						s = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(s, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						viewport_width: 0,
						viewport_height: 0,
						scroll_top: 0,
						search_results: n.props.default_search_results,
						search_from: 0,
						page_size: 48,
						is_more_results_available: !0,
						search_text: "",
						delayedPerformSearch: null,
						search_filter_search_by: "all",
						search_filter_order_by: "upload-date",
						search_filter_brands: [],
						current_page: 0,
						max_page: 1,
						is_page_initialized: !1,
						is_loading: !1,
						is_settings_active: !1,
						is_search_bar_active: !1,
						search_options_search_by: [{
							text: "All",
							slug: "all",
							is_active: !0
						}, {
							text: "Title",
							slug: "title",
							is_active: !1
						}, {
							text: "Tags",
							slug: "tags",
							is_active: !1
						}, {
							text: "Description",
							slug: "description",
							is_active: !1
						}],
						search_options_brands: n.getBrands(),
						search_options_order_by: [{
							text: "Upload Date",
							slug: "created_at",
							is_active: !0
						}, {
							text: "Views",
							slug: "views",
							is_active: !1
						}, {
							text: "Favorites",
							slug: "favorites_count",
							is_active: !1
						}, {
							text: "Release Date",
							slug: "released_at",
							is_active: !1
						}, {
							text: "Alphabetical",
							slug: "name.raw",
							is_active: !1
						}]
					}, n
				}
				return o(a, t), c(a, [{
					key: "componentDidMount",
					value: function() {
						var e = this;
						this.setupEventHandling(), this.updatePositionFromTop(), this.updateViewportDimensions(), $(".search-input").val(""), window.bLazy = new Blazy({}), $(".tse-scrollable").TrackpadScrollEmulator({
							wrapContent: !0,
							audoHide: !0
						}), this.setState({
							delayedPerformSearch: _.debounce(function(t) {
								e.performSearch(t)
							}, 300, {
								trailing: !0
							}),
							search_text: "",
							is_page_initialized: !0
						}, function() {
							setTimeout(function() {
								bLazy.revalidate()
							}, 200)
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						window.addEventListener("resize", _.debounce(this.updateViewportDimensions, 500, {
							trailing: !0
						}), !1), window.addEventListener("scroll", _.debounce(this.updatePositionFromTop, 150, {
							leading: !0,
							trailing: !0
						}), !1), App.events.addListener("TOGGLE_SETTINGS", function() {
							e.setState({
								is_settings_active: !e.state.is_settings_active
							})
						}), App.events.addListener("TOGGLE_SEARCH_BAR", function() {
							var t = !e.state.is_search_bar_active;
							e.setState({
								is_search_bar_active: t
							}), t && $("#search_input").focus()
						}), App.events.addListener("SEARCH_FILTER_ON_BRAND_CHANGE", function(t) {
							e.updateBrandFacetFilters(t.items)
						}), App.events.addListener("UPDATE_SORT_BY", function(t) {
							e.onOrderByChange(t.index)
						})
					}
				}, {
					key: "updateViewportDimensions",
					value: function() {
						this.setState({
							viewport_width: $(window).width(),
							viewport_height: $(window).height()
						})
					}
				}, {
					key: "getBrands",
					value: function() {
						var e = [],
							t = ["Almond Collective", "Amour", "Animac", "Arms", "Blue Eyes", "Bootleg", "BreakBottle", "Bunnywalker", "Celeb", "ChiChinoya", "ChuChu", "Circle Tribute", "CoCoans", "Collaboration Works", "Cranberry", "D3", "Daiei", "demodemon", "Digital Works", "Discovery", "EBIMARU-DO", "Echo", "Edge", "Erozuki", "evee", "FINAL FUCK 7", "Front Line", "GOLD BEAR", "Green Bunny", "Hoods Entertainment", "Hot Bear", "Hykobo", "Jellyfish", "kate_sai", "KENZsoft", "King Bee", "L.", "Lemon Heart", "Lune Pictures", "Magin Label", "Marigold", "Mary Jane", "MediaBank", "Moonstone Cherry", "MS Pictures", "Nihikime no Dozeu", "NuTech Digital", "@ OZ", "Pashmina", "Pinkbell", "Pink Pineapple", "Pixy Soft", "Pocomo Premium", "PoRO", "Project No.9", "Queen Bee", "Rabbit Gate", "SANDWICHWORKS", "Schoolzone", "Shinyusha", "Soft on Demand", "Studio 9 Maiami", "Studio Akai Shohosen", "Studio Deen", "Studio Fantasia", "Studio FOW", "studio GGB", "Suzuki Mirano", "SYLD", "TOHO", "Toranoana", "T-Rex", "TYS Work", "Umemaro-3D", "Union Cho", "Valkyria", "Vanilla", "White Bear", "yosino", "Y.O.U.C.", "ZIZ"],
							a = _.map(t, function(e) {
								return {
									text: e,
									slug: e,
									is_active: !1
								}
							});
						return e = e.concat(a)
					}
				}, {
					key: "updatePositionFromTop",
					value: function(e) {
						var t = 700,
							a = $(window).scrollTop(),
							n = $(document).height(),
							s = this.state.viewport_height,
							i = n - (a + s);
						this.setState({
							scroll_top: a
						}), this.state.is_page_initialized && !this.state.is_loading && t >= i && this.state.is_more_results_available && a > 0 && this.nextPage()
					}
				}, {
					key: "searchInputUpdate",
					value: function(e) {
						var t = this,
							a = e.target.value;
						window.scrollTo(0, 0), this.setState({
							search_text: a,
							search_from: 0
						}, function() {
							t.state.delayedPerformSearch(a)
						})
					}
				}, {
					key: "performSearch",
					value: function(t) {
						var a = this,
							n = arguments.length <= 1 || void 0 === arguments[1] ? {} : arguments[1],
							s = !!n.search_from,
							i = n.search_from || this.state.search_from;
						t != this.state.search_text && (i = 0, s = !1);
						var r = _.find(this.state.search_options_order_by, {
							is_active: !0
						});
						t = t.toLowerCase().replace(/[^a-z0-9 ]/g, ""), $.ajax(this.props.env.search_v2_base_url, {
							method: "POST",
							data: {
								q: t,
								search_by: this.state.search_filter_search_by,
								brands: this.state.search_filter_brands,
								sort_by: r.slug,
								sort_by_ordering: "desc",
								search_from: i,
								page_size: this.state.page_size
							},
							success: function(e) {
								l("Search result:", e), a.searchCallback(e, {
									is_next_page_content: s
								})
							},
							error: function(t) {
								e(t)
							}
						})
					}
				}, {
					key: "searchCallback",
					value: function(e) {
						var t = arguments.length <= 1 || void 0 === arguments[1] ? {} : arguments[1],
							a = e.hits;
						t.is_next_page_content && (a = this.state.search_results.concat(a)), this.setState({
							search_results: a,
							is_more_results_available: a.length < e.total,
							is_loading: !1
						}, function() {
							bLazy.revalidate()
						})
					}
				}, {
					key: "nextPage",
					value: function() {
						var e = this,
							t = this.state.search_from + this.state.page_size;
						l("Doing next page w/ search from:", t), this.setState({
							is_loading: !0,
							search_from: t
						}, function() {
							e.performSearch(e.state.search_text, {
								search_from: t
							})
						})
					}
				}, {
					key: "onKeyUp",
					value: function(e) {
						13 == e.which && ($(e.target).blur(), this.performSearch(e.target.value))
					}
				}, {
					key: "resetSearchInput",
					value: function(e, t) {
						var a = this;
						$(t).val("").focus(), this.setState({
							search_text: "",
							search_from: 0
						}, function() {
							a.performSearch("")
						})
					}
				}, {
					key: "onSearchByChange",
					value: function(e) {
						var t = this,
							a = _.clone(this.state.search_options_search_by);
						_.each(a, function(e) {
							e.is_active = !1
						});
						var n = a[e];
						n.is_active = !0, this.setState({
							search_options_search_by: a,
							search_filter_search_by: n.slug,
							current_page: 0,
							search_from: 0
						}, function() {
							t.performSearch(t.state.search_text)
						})
					}
				}, {
					key: "onOrderByChange",
					value: function(e) {
						var t = this,
							a = _.clone(this.state.search_options_order_by);
						_.each(a, function(e) {
							e.is_active = !1
						});
						var n = a[e];
						n.is_active = !0, this.setState({
							search_options_order_by: a,
							search_filter_order_by: n.slug,
							current_page: 0,
							search_from: 0
						}, function() {
							t.performSearch(t.state.search_text)
						})
					}
				}, {
					key: "updateBrandFacetFilters",
					value: function(e) {
						var t = this,
							a = [];
						_.each(e, function(e) {
							e.is_active && a.push(e.slug)
						}), this.setState({
							search_filter_brands: a,
							current_page: 0,
							search_from: 0
						}, function() {
							t.performSearch(t.state.search_text)
						})
					}
				}, {
					key: "toggleSettings",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), App.events.emit("TOGGLE_SETTINGS"), !1
					}
				}, {
					key: "getSelectedBrandsCount",
					value: function() {
						var e = _.filter(this.state.search_options_brands, {
							is_active: !0
						});
						return 0 == e.length ? this.state.search_options_brands.length : e.length
					}
				}, {
					key: "getUrl",
					value: function(e) {
						return "/hentai-videos/" + e.slug + "?r=/search"
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: classNames("search", {
								noscroll: this.state.is_settings_active
							})
						}, React.createElement(d["default"], this.props, React.createElement("div", {
							className: "flex mobile-header-nav-item"
						}), React.createElement("div", {
							className: "icon mobile-header-nav-item growing-icon",
							onTouchStart: function(e) {
								App.events.emit("TOGGLE_SEARCH_BAR")
							},
							onMouseDown: function(e) {
								App.events.emit("TOGGLE_SEARCH_BAR")
							}
						}, React.createElement("em", {
							className: "fa fa-search"
						})), React.createElement("div", {
							className: "icon mobile-header-nav-item growing-icon",
							onTouchStart: this.toggleSettings,
							onMouseDown: this.toggleSettings
						}, React.createElement("em", {
							className: "fa fa-cog"
						}))), React.createElement("div", {
							className: classNames("search-bar-mobile", {
								active: this.state.is_search_bar_active
							})
						}, React.createElement("div", {
							className: "icon growing-icon",
							onClick: function(e) {
								App.events.emit("TOGGLE_SEARCH_BAR")
							}
						}, React.createElement("em", {
							className: "fa fa-angle-left"
						})), React.createElement("div", {
							className: classNames("faux-placeholder-text", {
								active: 0 == this.state.search_text.length
							})
						}, "Search hanime.tv"), React.createElement("input", {
							id: "search_input",
							className: "search-input",
							type: "text",
							onChange: this.searchInputUpdate,
							onKeyUp: this.onKeyUp
						}), React.createElement("div", {
							className: classNames("reset-search-input growing-icon", {
								active: this.state.search_text.length > 0 && this.state.is_search_bar_active
							}),
							onClick: function(t) {
								e.resetSearchInput(t, "#search_input")
							}
						}, "×")), React.createElement("div", {
							className: "search-bar-tablet-plus"
						}, React.createElement("div", {
							className: "search-icon"
						}, React.createElement("em", {
							className: "fa fa-search"
						})), React.createElement("div", {
							className: classNames("faux-placeholder-text", {
								active: 0 == this.state.search_text.length
							})
						}, "Search hanime.tv"), React.createElement("input", {
							id: "search_input_tablet_plus",
							className: "search-input",
							type: "text",
							onChange: this.searchInputUpdate,
							onKeyUp: this.onKeyUp
						}), React.createElement("div", {
							className: "search-actions-container"
						}, React.createElement("div", {
							className: classNames("reset-search-input growing-icon", {
								active: this.state.search_text.length > 0
							}),
							onClick: function(t) {
								e.resetSearchInput(t, "#search_input_tablet_plus")
							}
						}, React.createElement("em", {
							className: "fa fa-close"
						})), React.createElement(b["default"], {
							className: "sort-by",
							items: this.state.search_options_order_by,
							on_select_event_name: "UPDATE_SORT_BY"
						}, React.createElement("div", {
							className: "selected-item"
						}, _.find(this.state.search_options_order_by, {
							is_active: !0
						}).text), React.createElement("em", {
							className: "fa fa-angle-down"
						})))), React.createElement("div", {
							className: "filters"
						}, React.createElement("div", {
							className: "filters-scroll-container tse-scrollable"
						}, React.createElement("div", {
							className: "tse-content"
						}, React.createElement("div", {
							className: "filler"
						}), React.createElement("div", {
							className: "section"
						}, React.createElement("div", {
							className: "section-heading"
						}, React.createElement("div", {
							className: "section-title"
						}, "Search By"), React.createElement("div", {
							className: "section-hint"
						}, this.state.search_options_search_by.length - 1)), React.createElement("div", {
							className: "section-content"
						}, React.createElement("div", {
							className: "radio-group inverse"
						}, _.map(this.state.search_options_search_by, function(t, a) {
							return React.createElement("div", {
								key: a,
								className: "radio-container"
							}, React.createElement("input", {
								type: "radio",
								name: "search_by",
								id: "search_by" + a,
								value: t.slug,
								checked: e.state.search_filter_search_by == t.slug,
								onChange: function(t) {
									e.onSearchByChange(a)
								}
							}), React.createElement("label", {
								htmlFor: "search_by" + a,
								className: classNames({
									active: e.state.search_filter_search_by == t.slug
								})
							}, React.createElement("em", {
								className: classNames("fa", e.state.search_filter_search_by == t.slug ? "fa-dot-circle-o" : "fa-circle-o")
							}), React.createElement("span", null, t.text)))
						})))), React.createElement("div", {
							className: "section"
						}, React.createElement("div", {
							className: "section-heading"
						}, React.createElement("div", {
							className: "section-title"
						}, "Brands"), React.createElement("div", {
							className: "section-hint"
						}, this.getSelectedBrandsCount())), React.createElement("div", {
							className: "section-content"
						}, React.createElement(g["default"], {
							options: this.state.search_options_brands,
							on_change_event_name: "SEARCH_FILTER_ON_BRAND_CHANGE",
							is_inverse: !0,
							is_display_all: !0
						})))))), React.createElement("div", {
							className: classNames("settings", {
								active: this.state.is_settings_active
							})
						}, React.createElement("div", {
							className: "settings-header"
						}, React.createElement("div", {
							className: "icon growing-icon",
							onClick: function(e) {
								App.events.emit("TOGGLE_SETTINGS")
							}
						}, React.createElement("em", {
							className: "fa fa-angle-left"
						})), React.createElement("div", {
							className: "settings-header-title"
						}, "Settings")), React.createElement("div", {
							className: "settings-content-container tse-scrollable"
						}, React.createElement("div", {
							className: "settings-content tse-content"
						}, React.createElement("div", {
							className: "section"
						}, React.createElement("div", {
							className: "section-title"
						}, "Search Filters"), React.createElement("div", {
							className: "subsection"
						}, React.createElement("div", {
							className: "subsection-title"
						}, "Search By"), React.createElement("div", {
							className: "subsection-content"
						}, React.createElement("div", {
							className: "radio-group"
						}, _.map(this.state.search_options_search_by, function(t, a) {
							return React.createElement("div", {
								key: a,
								className: "radio-container"
							}, React.createElement("input", {
								type: "radio",
								name: "search_by",
								id: "search_by" + a,
								value: t.slug,
								checked: e.state.search_filter_search_by == t.slug,
								onChange: function(t) {
									e.onSearchByChange(a)
								}
							}), React.createElement("label", {
								htmlFor: "search_by" + a
							}, React.createElement("em", {
								className: classNames("fa", e.state.search_filter_search_by == t.slug ? "fa-dot-circle-o" : "fa-circle-o")
							}), React.createElement("span", null, t.text)))
						})))), React.createElement("div", {
							className: "subsection"
						}, React.createElement("div", {
							className: "subsection-title"
						}, "Brands / Production Studio"), React.createElement("div", {
							className: "subsection-content"
						}, React.createElement(g["default"], {
							options: this.state.search_options_brands,
							on_change_event_name: "SEARCH_FILTER_ON_BRAND_CHANGE"
						})))), React.createElement("div", {
							className: "section"
						}, React.createElement("div", {
							className: "section-title"
						}, "Search Results Ordering"), React.createElement("div", {
							className: "subsection"
						}, React.createElement("div", {
							className: "subsection-title"
						}, "Sort By"), React.createElement("div", {
							className: "subsection-content"
						}, React.createElement("div", {
							className: "radio-group"
						}, _.map(this.state.search_options_order_by, function(t, a) {
							return React.createElement("div", {
								key: a,
								className: "radio-container"
							}, React.createElement("input", {
								type: "radio",
								name: "order_by",
								id: "order_by" + a,
								value: t.slug,
								checked: e.state.search_filter_order_by == t.slug,
								onChange: function(t) {
									e.onOrderByChange(a)
								}
							}), React.createElement("label", {
								htmlFor: "order_by" + a
							}, React.createElement("em", {
								className: classNames("fa", e.state.search_filter_order_by == t.slug ? "fa-dot-circle-o" : "fa-circle-o")
							}), React.createElement("span", null, t.text)))
						})))))))), React.createElement("div", {
							className: "content flex-col"
						}, React.createElement("div", {
							className: "flex-row justify-center"
						}, React.createElement(w["default"], {
							className: "",
							id: "search_banner_top",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width
						})), this.state.search_results && 0 != this.state.search_results.length ? React.createElement("div", {
							className: "search-results"
						}, React.createElement(N["default"], {
							className: "flex-row justify-center align-center transition-all",
							scroll_top: this.state.scroll_top,
							scroll_top_start: 1,
							scroll_top_end: 3e3,
							size: "desktop",
							viewport_width: this.state.viewport_width
						}, React.createElement(w["default"], {
							className: "adjustment-placeholder",
							id: "search_banner_1",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width,
							scroll_top: this.state.scroll_top
						})), React.createElement(N["default"], {
							className: "flex-row justify-center align-center transition-all",
							scroll_top: this.state.scroll_top,
							scroll_top_start: 1,
							scroll_top_end: 3e3,
							size: "tablet",
							viewport_width: this.state.viewport_width
						}, React.createElement(w["default"], {
							className: "adjustment-placeholder",
							id: "search_banner_1",
							is_ads_enabled: this.props.is_ads_enabled,
							viewport_width: this.state.viewport_width,
							scroll_top: this.state.scroll_top
						})), _.map(this.state.search_results, function(t, a) {
							return React.createElement("a", {
								className: "search-result",
								key: t.id + "_" + a,
								href: e.getUrl(t),
								title: "Watch " + t.name + " video in HD"
							}, React.createElement("img", {
								className: "b-lazy b-lazy-pop-in",
								src: App.transparent,
								"data-src": t.cover_url,
								alt: t.name + " cover image",
								width: "100%"
							}), React.createElement("div", {
								className: "title"
							}, t.name))
						})) : React.createElement("div", {
							className: "no-search-results"
						}, "No search results. =(")), React.createElement("div", {
							className: classNames("loading", {
								active: this.state.is_loading
							})
						}, React.createElement("em", {
							className: "fa fa-spinner fa-spin"
						})), React.createElement(h["default"], null), React.createElement(f["default"], null))
					}
				}]), a
			}(React.Component);
		a["default"] = k
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(1),
			l = n(c),
			u = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						form: {
							name: "",
							email: "",
							password: "",
							password_confirmation: "",
							remember_me: "1",
							user_agent: "",
							screen_width: "",
							screen_height: "",
							operating_system: ""
						},
						is_submitting: !1,
						status_text: ""
					}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.state.form.user_agent = navigator.userAgent, this.state.form.screen_width = screen.width, this.state.form.screen_height = screen.height, this.state.form.operating_system = jscd.os + " " + jscd.osVersion, $("#name").focus()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "register",
					value: function() {
						var e = this;
						this.isRegisterButtonEnabled() && (this.setState({
							is_submitting: !0
						}), $.post("/api/v1/users", {
							user: this.state.form
						}).done(function(t) {
							e.setState({
								status_text: ""
							}), window.location = window.location.protocol + "//" + window.location.hostname + ":" + window.location.port
						}).fail(function(t) {
							var a = t.statusText;
							t.responseJSON && (a = t.responseJSON.errors), e.setState({
								status_text: a,
								is_submitting: !1
							})
						}).always(function() {}))
					}
				}, {
					key: "updateForm",
					value: function(e, t) {
						var a = this.state.form;
						a[t] = e.target.value, this.setState({
							form: a
						})
					}
				}, {
					key: "isRegisterButtonEnabled",
					value: function() {
						return 0 == this.state.form.name.length ? !1 : "undefined" == typeof this.state.form.email || 0 == this.state.form.email.length ? !1 : this.state.form.password.length < 6 ? !1 : 0 == this.state.form.password_confirmation.length ? !1 : this.state.form.password != this.state.form.password_confirmation ? !1 : App.isValidEmail(this.state.form.email) ? !this.state.is_submitting : !1
					}
				}, {
					key: "handleNext",
					value: function(e, t, a) {
						13 == e.which && ("register" == a ? this.register() : $(t).focus())
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: "sign-up has-bg"
						}, React.createElement(l["default"], this.props), React.createElement("div", {
							className: "panel"
						}, React.createElement("div", {
							className: "panel-section"
						}, React.createElement("div", {
							className: "ribbon ribbon-small ribbon-orange"
						}, React.createElement("div", {
							className: "banner"
						}, React.createElement("h2", {
							className: "text"
						}, React.createElement("em", {
							className: "fa fa-lock"
						}), "  SSL"))), React.createElement("a", {
							href: "/"
						}, React.createElement("img", {
							src: "logo-100.png",
							className: "logo",
							alt: "Free Anime Hentai HD Streams for Mobile"
						})), React.createElement("h1", null, "Create Account"), React.createElement("input", {
							className: "input-responsive",
							id: "name",
							type: "text",
							placeholder: "Username",
							onChange: function(t) {
								e.updateForm(t, "name")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "#email")
							}
						}), React.createElement("input", {
							className: "input-responsive",
							id: "email",
							type: "email",
							placeholder: "Email Address",
							onChange: function(t) {
								e.updateForm(t, "email")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "#password")
							}
						}), React.createElement("input", {
							className: "input-responsive",
							id: "password",
							type: "password",
							placeholder: "Password (6+ characters)",
							onChange: function(t) {
								e.updateForm(t, "password")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "#password_confirmation")
							}
						}), React.createElement("input", {
							className: "input-responsive",
							id: "password_confirmation",
							type: "password",
							placeholder: "Password Confirm",
							onChange: function(t) {
								e.updateForm(t, "password_confirmation")
							},
							onKeyUp: function(t) {
								e.handleNext(t, "", "register")
							}
						}), this.state.status_text ? React.createElement("div", {
							className: "status-text"
						}, this.state.status_text) : null, React.createElement("div", {
							className: "row"
						}, React.createElement("div", {
							className: "col-1"
						}, React.createElement("button", {
							className: classNames("button button-primary button-sm button-responsive", {
								disabled: !this.isRegisterButtonEnabled()
							}),
							onClick: this.register
						}, this.state.is_submitting ? React.createElement("span", null, React.createElement("em", {
							className: "fa fa-spinner fa-spin"
						})) : React.createElement("span", null, "Create Free Account"))), React.createElement("div", {
							className: "col-2"
						}, React.createElement("a", {
							href: "/",
							className: "button button-sm button-responsive"
						}, "Cancel")))), React.createElement("div", {
							className: "panel-section panel-section-dark"
						}, React.createElement("div", {
							className: "panel-text"
						}, "Already a member?"), React.createElement("a", {
							href: "/log-in",
							className: "button button-sm button-responsive"
						}, "Log In"))))
					}
				}]), t
			}(React.Component);
		t["default"] = u
	}, function(t, a, n) {
		"use strict";

		function s(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function i(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function r(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function o(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(a, "__esModule", {
			value: !0
		});
		var c = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			u = n(34),
			d = s(u),
			p = function(t) {
				function a(e, t) {
					i(this, a);
					var n = r(this, Object.getPrototypeOf(a).call(this, e, t)),
						s = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(s, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						hentai_video: {
							is_censored: !0,
							is_hard_subtitled: !0,
							tags: [],
							manual_tags: ""
						},
						cached_hentai_video: {
							is_censored: !0,
							is_hard_subtitled: !0,
							tags: [],
							manual_tags: ""
						},
						pending_hentai_franchise_bind: null,
						transcodes: [],
						tag_search_results: {
							hh: [],
							hentaipulse: [],
							hentairon: [],
							hentaiddl: [],
							muchohentai: [],
							hentaistreaming: []
						},
						selected_tag_search_results: {
							hh: [],
							hentaipulse: [],
							hentairon: [],
							hentaiddl: [],
							muchohentai: [],
							hentaistreaming: []
						},
						cover_url_drop_active: !1,
						cover_url_drop_percentage: 0,
						poster_url_drop_active: !1,
						poster_url_drop_percentage: 0,
						is_loading: !1,
						hentai_video_storyboards: []
					}, n
				}
				return o(a, t), c(a, [{
					key: "componentDidMount",
					value: function() {
						var t = this;
						this.setupEventHandling(), window.bLazy = new Blazy;
						var a = this;
						filepicker.setKey(this.props.env.filestack_api_key), filepicker.makeDropPane($("#cover_url_drag_drop_pane")[0], {
							multiple: !1,
							dragEnter: function() {
								a.setState({
									cover_url_drop_active: !0
								})
							},
							dragLeave: function() {
								a.setState({
									cover_url_drop_active: !1
								})
							},
							onSuccess: function(e) {
								l(JSON.stringify(e));
								var t = e[0],
									n = _.clone(a.state.hentai_video);
								n.cover_url = t.url, a.setState({
									hentai_video: n,
									cover_url_drop_active: !1
								})
							},
							onError: function(t, a) {
								e("(" + t + ") " + a)
							},
							onProgress: function(e) {
								a.setState({
									cover_url_drop_percentage: e
								})
							}
						}), filepicker.makeDropPane($("#poster_url_drag_drop_pane")[0], {
							multiple: !1,
							dragEnter: function() {
								a.setState({
									poster_url_drop_active: !0
								})
							},
							dragLeave: function() {
								a.setState({
									poster_url_drop_active: !1
								})
							},
							onSuccess: function(e) {
								l(JSON.stringify(e));
								var t = e[0],
									n = _.clone(a.state.hentai_video);
								n.poster_url = t.url, a.setState({
									hentai_video: n,
									poster_url_drop_active: !1
								})
							},
							onError: function(t, a) {
								e("(" + t + ") " + a)
							},
							onProgress: function(e) {
								a.setState({
									poster_url_drop_percentage: e
								})
							}
						}), $.ajax("/api/v2/transcodes", {
							method: "GET",
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								t.setState({
									transcodes: e
								}, function() {
									$(".tse-scrollable").TrackpadScrollEmulator({
										wrapContent: !0,
										autoHide: !1
									})
								})
							}
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						App.events.addListener("HENTAI_FRANCHISE_SELECTED", function(t) {
							e.setState({
								pending_hentai_franchise_bind: t.hentai_franchise
							})
						})
					}
				}, {
					key: "onEnter",
					value: function(e, t) {
						13 == e.which && ($(e.target).blur(), t())
					}
				}, {
					key: "findHentaiVideo",
					value: function(t, a) {
						var n = this;
						a || (a = $("#hv_search_input").val()), $.ajax({
							type: "GET",
							url: "/api/v2/hentai_videos/" + a,
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								l(e), n.setState({
									hentai_video: e,
									cached_hentai_video: e
								}, function() {
									bLazy.revalidate()
								}), $("#hv_search_input").val(e.slug);
								var t = $.trim(e.name.replace(/\d/, "").split().join(""));
								$("#search_input").val(t), App.events.emit("SEARCH_HENTAI_FRANCHISE", {
									name: t
								})
							},
							error: function(t) {
								e(t)
							}
						})
					}
				}, {
					key: "findNextHentaiVideo",
					value: function(e) {
						var t = this.state.hentai_video;
						t && this.findHentaiVideo(e, t.id + 1)
					}
				}, {
					key: "bindHentaiFranchiseToHentaiVideo",
					value: function(t, a) {
						var n = this;
						if (a.id) $.ajax({
							type: "PUT",
							url: "/api/v2/hentai_videos/" + a.id,
							data: {
								hentai_video: {
									hentai_franchise_id: t.id
								}
							},
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								l(e), n.setState({
									hentai_video: e
								})
							},
							error: function(t) {
								e(t)
							}
						});
						else {
							var s = _.clone(this.state.hentai_video);
							s.hentai_franchise_id = t.id, this.setState({
								hentai_video: s
							})
						}
					}
				}, {
					key: "verifyBindHentaiFranchise",
					value: function(e) {
						var t = this.state.pending_hentai_franchise_bind,
							a = this.state.hentai_video,
							n = confirm("Bind " + t.title + " to " + a.name + "?");
						n && this.bindHentaiFranchiseToHentaiVideo(t, a)
					}
				}, {
					key: "isAbleToCreateHentaiVideo",
					value: function() {
						var e = this.state.hentai_video;
						return _.isEmpty(e) ? !1 : e.name && 0 != e.name.length && e.cover_url && e.poster_url && e.hentai_franchise_id ? !this.state.is_loading : !1
					}
				}, {
					key: "handleNext",
					value: function(e, t, a) {
						13 == e.which && ("x" == a ? l("x") : $(t).focus())
					}
				}, {
					key: "updateFieldDb",
					value: function(t) {
						var a = this;
						this.setState({
							is_loading: !0
						});
						var n = this.state.hentai_video,
							s = {
								hentai_video: {}
							};
						"video_id" == t ? (s[t] = n[t], s.hentai_video.id = n.id) : s.hentai_video[t] = n[t], $.ajax("/api/v2/hentai_videos/" + n.id, {
							method: "PUT",
							headers: {
								"X-Directive": "api"
							},
							data: s,
							success: function(e) {
								l(e), a.setState({
									cached_hentai_video: n,
									is_loading: !1
								})
							},
							error: function(t) {
								e(t), a.setState({
									is_loading: !1
								})
							}
						})
					}
				}, {
					key: "updateField",
					value: function(e, t) {
						var a = _.clone(this.state.hentai_video);
						a[e] = t, this.setState({
							hentai_video: a
						})
					}
				}, {
					key: "updateFields",
					value: function(e, t) {
						var a = _.clone(this.state.hentai_video);
						_.each(e, function(e) {
							a[e] = t
						}), this.setState({
							hentai_video: a
						})
					}
				}, {
					key: "selectTranscode",
					value: function(e, t) {
						var a = _.clone(this.state.hentai_video);
						a.video_id = t.id, a.sample_poster_url = t.thumbnail_url, this.setState({
							hentai_video: a
						})
					}
				}, {
					key: "searchSites",
					value: function(t, a) {
						var n = this;
						this.setState({
							is_loading: !0
						}), $.ajax("/api/v2/boba_fetch", {
							method: "POST",
							data: {
								site_name: a,
								search_term: this.state.hentai_video.tag_term
							},
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								var t = _.clone(n.state.tag_search_results);
								t[a] = e, n.setState({
									tag_search_results: t,
									is_loading: !1
								})
							},
							error: function(t) {
								e(t), n.setState({
									is_loading: !1
								})
							}
						})
					}
				}, {
					key: "toggleTagSearchResult",
					value: function(t, a, n) {
						var s = this,
							i = _.clone(this.state.selected_tag_search_results);
						0 == i[a].length ? (i[a] = n, "hh" == a ? this.setState({
							selected_tag_search_results: i
						}) : $.ajax("/api/v2/boba_fetch/scrape_for_tags", {
							method: "POST",
							data: {
								site_name: a,
								url: n.url
							},
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								n.tags = e, i[a] = n, s.setState({
									selected_tag_search_results: i
								})
							},
							error: function(t) {
								e(t)
							}
						})) : (i[a] = [], this.setState({
							selected_tag_search_results: i
						}))
					}
				}, {
					key: "toggleClassActive",
					value: function(e) {
						var t = $(e.target);
						t.hasClass("tag") || (t = t.parent()), t.toggleClass("active")
					}
				}, {
					key: "tagsPool",
					value: function() {
						var e = this,
							t = {};
						for (var a in this.state.selected_tag_search_results) {
							var n = this.state.selected_tag_search_results[a];
							n && _.each(n.tags, function(e) {
								t[e] = t[e] ? t[e] + 1 : 1
							})
						}
						return _.map(t, function(t, a) {
							return React.createElement("div", {
								key: a,
								className: "tag active",
								"data-tag": a,
								onClick: e.toggleClassActive
							}, a, " (", t, ")")
						})
					}
				}, {
					key: "createVideo",
					value: function() {
						var t = this;
						this.setState({
							is_loading: !0
						});
						var a = this.state.hentai_video,
							n = this.state.hentai_video.manual_tags.split("\n"),
							s = [],
							i = $(".tag.active");
						_.each(i, function(e) {
							s.push($(e).data("tag"))
						}), a.tags = n.concat(s), $.ajax("/api/v2/hentai_videos", {
							method: "POST",
							data: a,
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								l(e);
								var a = $.extend(t.state.hentai_video, e);
								t.setState({
									hentai_video: a,
									is_loading: !1
								}), alert("SUCCESS! New ID: " + e.id)
							},
							error: function(a) {
								e(a), t.setState({
									is_loading: !1
								})
							}
						})
					}
				}, {
					key: "commitManual",
					value: function() {
						var e = this.state.hentai_video.manual_tags.split("\n");
						this.commitWithTags(e)
					}
				}, {
					key: "commitSelectedTags",
					value: function() {
						var e = [],
							t = $(".tag.active");
						_.each(t, function(t) {
							e.push($(t).data("tag"))
						}), this.commitWithTags(e)
					}
				}, {
					key: "commitWithTags",
					value: function(t) {
						var a = this,
							n = this.state.hentai_video;
						this.setState({
							is_loading: !0
						}), $.ajax("/api/v2/hentai_videos/" + n.slug + "/hentai_tags", {
							method: "POST",
							headers: {
								"X-Directive": "api"
							},
							data: {
								hentai_tag: {
									action: "batch_add",
									tags: t
								}
							},
							success: function(e) {
								l(e), a.setState({
									is_loading: !1
								})
							},
							error: function(t) {
								e(t), a.setState({
									is_loading: !1
								})
							}
						})
					}
				}, {
					key: "reinitializeStoryboards",
					value: function() {
						var t = this;
						this.setState({
							is_loading: !0
						});
						var a = this.state.hentai_video;
						$.ajax("/api/v2/hentai_video_storyboards", {
							method: "POST",
							headers: {
								"X-Directive": "api"
							},
							data: {
								hentai_video_id: a.id
							},
							success: function(e) {
								l(e), t.setState({
									is_loading: !1,
									hentai_video_storyboards: e
								})
							},
							error: function(a) {
								e(a), t.setState({
									is_loading: !1
								})
							}
						})
					}
				}, {
					key: "render",
					value: function() {
						return d["default"].apply(this)
					}
				}]), a
			}(React.Component);
		a["default"] = p
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		

		
		
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(35),
			l = n(c),
			u = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						viewport_width: 0,
						viewport_height: 0,
						background_style: {
							backgroundImage: "url('" + n.props.video.poster_url + "')"
						},
						is_video_player_active: !1,
						video: n.props.video,
						hentai_video_favorites: n.props.hentai_video_favorites,
						favorite: n.getHentaiVideoFavorite(),
						is_error_loading_video_player: !1,
						is_play_analytics_sent: !1,
						is_showing_more_description: !1,
						is_more_description_visible: !1,
						transcodes: n.props.transcodes,
						storyboard_thumbnails: null,
						is_page_initialized: !1,
						is_download_supported: !1,
						is_touch_enabled: !1,
						is_ios: !1
					}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling(), this.onScreenResize(), window.bLazy = new Blazy({
							container: ".items-container"
						}), this.setState({
							is_page_initialized: !0,
							is_download_supported: "download" in document.createElement("a"),
							is_touch_enabled: Modernizr.touchevents,
							is_ios: /iPad|iPhone|iPod/.test(navigator.userAgent) && !window.MSStream,
							storyboard_thumbnails: this.generateStoryboardThumbnails()
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						window.addEventListener("resize", _.debounce(this.onScreenResize, 500, {
							leading: !0,
							trailing: !0
						})), App.events.addListener("htv-video-player-activate", function(t) {
							e.setState({
								is_video_player_active: !0
							})
						}), App.events.addListener("htv-video-player-deactivate", function(t) {
							e.setState({
								is_video_player_active: !1
							})
						}), App.events.addListener("favorite-created", this.favoriteCreated), App.events.addListener("favorite-destroyed", this.favoriteDestroyed), App.events.addListener("toggle-favorite-not-logged-in-prompt", function() {
							App.events.emit("MODAL_ACTIVATE", {
								title: "Login Required",
								type: "login-required-modal",
								body: "Adding this hentai episode to your favorites list requires logging in!"
							})
						}), App.events.addListener("HTV_VIDEO_PLAYER_ERROR", function(t) {
							e.setState({
								is_error_loading_video_player: !0
							}), App.events.emit("MODAL_ACTIVATE", {
								type: "video-player-error-modal",
								title: "Opps!",
								body: t.msg
							}), t.is_h264_supported || t.is_webm_supported || -1 != navigator.userAgent.indexOf("Googlebot") || -1 != navigator.userAgent.indexOf("bingbot") || $.ajax({
								type: "POST",
								url: "/api/v1/errors",
								data: {
									type: "HTVVideoPlayer Error :: ua: " + navigator.userAgent,
									msg: t.msg,
									is_h264_supported: t.is_h264_supported,
									is_webm_supported: t.is_webm_supported,
									current_url: window.location.href,
									transcode_url: t.transcode_url,
									w: $(window).width(),
									h: $(window).height()
								}
							})
						})
					}
				}, {
					key: "onScreenResize",
					value: function() {
						if (this.setState({
								viewport_width: window.innerWidth,
								viewport_height: window.innerHeight
							}), !this.state.is_showing_more_description) {
							var e = $("#description").height();
							e >= 180 ? this.setState({
								is_more_description_visible: !0
							}) : this.setState({
								is_more_description_visible: !1
							})
						}
					}
				}, {
					key: "favoriteDestroyed",
					value: function(e) {
						if (this.state.favorite) {
							var t = _.map(this.state.hentai_video_favorites, _.clone);
							_.remove(t, this.state.favorite);
							var a = _.clone(this.state.video);
							a.favorites_count--, this.setState({
								video: a,
								hentai_video_favorites: t,
								favorite: null
							})
						}
					}
				}, {
					key: "favoriteCreated",
					value: function(e) {
						var t = _.find(this.state.hentai_video_favorites, e.favorite);
						if ("undefined" == typeof t) {
							var a = _.map(this.state.hentai_video_favorites, _.clone);
							a.push(e.favorite);
							var n = _.clone(this.state.video);
							n.favorites_count++, this.setState({
								video: n,
								hentai_video_favorites: a,
								favorite: e.favorite
							})
						}
					}
				}, {
					key: "getHentaiVideoFavorite",
					value: function() {
						var e = this.props.hentai_video_favorites;
						this.state && (e = this.state.hentai_video_favorites);
						var t = _.filter(e, {
							hentai_video_id: this.props.video.id
						});
						return t.length > 0 ? t[0] : null
					}
				}, {
					key: "goBack",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.props.return_url ? window.location.href = window.location.protocol + "//" + window.location.host + this.props.return_url : window.location.href = window.location.protocol + "//" + window.location.host + "?cb=" + (new Date).getTime(), !1
					}
				}, {
					key: "doNothing",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), !1
					}
				}, {
					key: "emitActivateVideo",
					value: function(e) {
						App.events.emit("htv-video-player-activate", {}), App.analytics({
							type: "VIDEO_PLAY",
							endpoint: "/hentai_video_play",
							payload: {
								hentai_video_id: this.state.video.id
							}
						})
					}
				}, {
					key: "emitContactUsModalActivate",
					value: function(e) {
						App.events.emit("MODAL_ACTIVATE", {
							title: "Contact Us",
							type: "contact-us-modal",
							params: {
								is_h264_supported: this.state
							}
						})
					}
				}, {
					key: "emitDownloadWarning",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), App.events.emit("MODAL_ACTIVATE", {
							title: "Download Help",
							type: "warning-modal",
							body: "<p>1.) <a class='primary-color' href='https://web.archive.org/web/20170201123401/https://www.youtube.com/watch?v=sgWs9NxLzH8'>Right click</a> or <a class='primary-color' href='https://web.archive.org/web/20170201123401/https://www.youtube.com/watch?v=8Ly6wFCG7BQ'>Long-Press</a> on the button!</p><p>2.) Select Save Link As...</p><p>3.) Name your file.</p><p>4.) Click on Save.</p>",
							is_footer_visible: !1
						}), !1
					}
				}, {
					key: "showMoreDescription",
					value: function(e) {
						this.setState({
							is_showing_more_description: !0
						})
					}
				}, {
					key: "getUrl",
					value: function(e) {
						return "/hentai-videos/" + e.slug + "?r=/hentai-videos/" + this.state.video.slug
					}
				}, {
					key: "numPrimarySlidesCalculator",
					value: function(e) {
						var t = 2;
						return t = 500 > e ? 2 : 800 > e ? 3 : 1100 > e ? 4 : 1200 > e ? 5 : 1400 > e ? 3 : 1601 > e ? 4 : 5
					}
				}, {
					key: "generateStoryboardThumbnails",
					value: function() {
						if (this.props.hentai_video_storyboards && 0 != this.props.hentai_video_storyboards.length) {
							for (var e = function(e, t, a) {
									var n = t.num_horizontal_frames * t.num_vertical_frames,
										s = parseInt(Math.floor(e / n)),
										i = a[s],
										r = e % n,
										o = r % t.num_horizontal_frames,
										c = parseInt(r / t.num_horizontal_frames),
										l = o * t.frame_width,
										u = c * t.frame_height;
									return {
										width: t.frame_width + "px",
										height: t.frame_height + "px",
										background: "url('" + i.url + "') no-repeat",
										backgroundPosition: -l + "px " + -u + "px"
									}
								}, t = 12, a = this.props.hentai_video_storyboards, n = a[0], s = parseInt(Math.floor(n.num_total_frames / t)), i = parseInt(Math.ceil(s / 2)), r = [], o = 0; t > o; o++) {
								var c = i + o * s,
									l = e(c, n, a);
								r.push(l)
							}
							var u = React.createElement("div", {
								className: "flex-row flex-wrap"
							}, _.map(r, function(e, t) {
								return React.createElement("div", {
									className: "storyboard-thumbnail",
									style: e,
									key: t
								})
							}));
							return u
						}
					}
				}, {
					key: "download",
					value: function(e, t) {
						t.is_encoding || this.emitDownloadWarning(e)
					}
				}, {
					key: "downloadUrl",
					value: function(e) {
						return e.is_encoding ? e.cached_itag_url : e.cached_itag_url
					}
				}, {
					key: "downloadFilename",
					value: function(e) {
						return e.is_encoding ? this.props.video.slug + "-" + e.height + "p." + e.file_format_extension : this.props.video.slug + "-" + e.height + "p." + e.file_format_extension
					}
				}, {
					key: "render",
					value: function() {
						return l["default"].apply(this)
					}
				}]), t
			}(React.Component);
		t["default"] = u
	}, function(e, t, a) {
		(function(t) {
			"use strict";

			function a(e, a, n, s, i, r, o, c) {
				if ("production" !== t.env.NODE_ENV && void 0 === a) throw new Error("invariant requires an error message argument");
				if (!e) {
					var l;
					if (void 0 === a) l = new Error("Minified exception occurred; use the non-minified dev environment for the full error message and additional helpful warnings.");
					else {
						var u = [n, s, i, r, o, c],
							d = 0;
						l = new Error(a.replace(/%s/g, function() {
							return u[d++]
						})), l.name = "Invariant Violation"
					}
					throw l.framesToPop = 1, l
				}
			}
			e.exports = a
		}).call(t, a(9))
	}, function(e, t, a) {
		function n(e) {
			return a(s(e))
		}

		function s(e) {
			return i[e] || function() {
				throw new Error("Cannot find module '" + e + "'.")
			}()
		}
		var i = {
			"./Apps": 10,
			"./Apps.jsx": 10,
			"./Favorites": 11,
			"./Favorites.jsx": 11,
			"./ForgotPassword": 12,
			"./ForgotPassword.jsx": 12,
			"./Landing": 13,
			"./Landing.jsx": 13,
			"./LogIn": 14,
			"./LogIn.jsx": 14,
			"./ResetPassword": 15,
			"./ResetPassword.jsx": 15,
			"./Search": 16,
			"./Search.jsx": 16,
			"./SignUp": 17,
			"./SignUp.jsx": 17,
			"./VideoManager": 18,
			"./VideoManager.jsx": 18,
			"./VideoShow": 19,
			"./VideoShow.jsx": 19
		};
		n.keys = function() {
			return Object.keys(i)
		}, n.resolve = s, e.exports = n, n.id = 21
	}, function(e, t, a) {
		(function(n) {
			"use strict";
			Object.defineProperty(t, "__esModule", {
				value: !0
			});
			var s = a(36),
				i = s.EventEmitter,
				r = function(t) {
					var s = "undefined" != typeof e && e.exports,
						i = null;
					i = s ? n : window;
					var r = i[t.layout];
					return r || (r = i[t.layout] = a(21)("./" + t.layout)["default"]), React.createFactory(r)(t)
				};
			r.transparent = "data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==", r.isIOS = function() {
				return /iPad|iPhone|iPod/.test(navigator.userAgent) && !window.MSStream
			}, r.isValidEmail = function(e) {
				var t = /^(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
				return t.test(e)
			}, r.datetimeToHuman = function(e) {
				var t = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
					a = new Date(Date.parse(e));
				return t[a.getMonth()] + " " + a.getDate() + ", " + a.getUTCFullYear()
			}, r.addCommasToNumber = function(e) {
				var t = parseInt(e).toLocaleString("en"),
					a = t.indexOf(".");
				return 0 > a ? t : t.substring(0, t.indexOf("."))
			}, r.secondsToHuman = function(e) {
				var t = arguments.length <= 1 || void 0 === arguments[1] ? {} : arguments[1];
				if (isNaN(e)) return "";
				var a = parseInt(e / 3600) % 24,
					n = parseInt(e / 60) % 60,
					s = parseInt(e % 60);
				return t.indicators ? a > 0 ? a + "h " + (10 > n ? "0" + n : n) + "m " + (10 > s ? "0" + s : s) + "s" : n + "m " + (10 > s ? "0" + s : s) + "s" : a > 0 ? a + ":" + (10 > n ? "0" + n : n) + ":" + (10 > s ? "0" + s : s) : n + ":" + (10 > s ? "0" + s : s)
			}, r.doNothing = function(e) {
				return e.preventDefault(), e.stopPropagation(), !1
			}, r.cssAnimationEvent = function(e, t, a) {
				for (var n = ["webkit", "moz", "MS", "o", ""], s = 0; s < n.length; s++) n[s] || (t = t.toLowerCase()), e.addEventListener(n[s] + t, a, !1)
			}, r.analytics = function(e) {
				$.ajax({
					type: "POST",
					url: e.endpoint,
					data: e.payload
				})
			}, r.events = new i, r.emit = function(e, t) {
				r.events.emit(e, t)
			}, t["default"] = r
		}).call(t, function() {
			return this
		}())
	}, function(e, t, a) {
		(function(e) {
			"use strict";

			function t(e) {
				return e && e.__esModule ? e : {
					"default": e
				}
			}
			var n = a(22),
				s = t(n);
			"undefined" != typeof window ? (window.App = s["default"], window.l = console.log.bind(console), window.e = console.error.bind(console), document.addEventListener("DOMContentLoaded", function() {
				var e = water,
					t = document.getElementById("render_target");
				ReactDOM.render((0, s["default"])(e), t)
			})) : (e.App = s["default"], e.l = console.log.bind(console), e.e = console.error.bind(console))
		}).call(t, function() {
			return this
		}())
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: "navbar"
						}, React.createElement("ul", {
							className: "nav nav-pills nav-stacked"
						}, React.createElement("li", {
							role: "presentation",
							className: classNames({
								active: "Landing" == this.props.layout
							})
						}, React.createElement("a", {
							href: "#"
						}, "HTV2 Video Manager")), React.createElement("li", {
							className: "",
							role: "presentation"
						}, React.createElement("a", {
							href: "#"
						}, "HTV Franchise 2")), React.createElement("li", {
							className: "",
							role: "presentation"
						}, React.createElement("a", {
							href: "#"
						}, "HTV Franchise 3"))))
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			var a = {};
			for (var n in e) t.indexOf(n) >= 0 || Object.prototype.hasOwnProperty.call(e, n) && (a[n] = e[n]);
			return a
		}

		function n(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function s(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function i(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var r = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			o = [750, 19],
			c = [600, 25],
			l = function(e) {
				function t(e, a) {
					n(this, t);
					var i = s(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						is_dropdown_menu_visible: !1,
						current_selected_height: 720
					}, i
				}
				return i(t, e), r(t, [{
					key: "componentDidMount",
					value: function() {
						var e = this;
						this.setupEventHandling(), App.events.addListener("htv-video-player-change-resolution", function(t) {
							e.changeResolution(t.height, t.url, t.autoplay)
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "showDropdown",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.setState({
							is_dropdown_menu_visible: !0
						}), document.addEventListener("click", this.hideDropdown), document.addEventListener("touchstart", this.hideDropdown), !1
					}
				}, {
					key: "hideDropdown",
					value: function() {
						this.setState({
							is_dropdown_menu_visible: !1
						}), document.removeEventListener("click", this.hideDropdown), document.removeEventListener("touchstart", this.hideDropdown)
					}
				}, {
					key: "enterStyles",
					value: function(e, t, a, n, s) {
						return {
							height: 0,
							opacity: 1,
							top: 0,
							data: this.props.items[e]
						}
					}
				}, {
					key: "styles",
					value: function() {
						if (!this.state.is_dropdown_menu_visible) return {};
						var e = this.props.items;
						return Object.keys(e).reduce(function(t, a) {
							return t[a] = {
								height: spring(42, o),
								opacity: spring(1, o),
								top: 0,
								data: e[a]
							}, t
						}, {})
					}
				}, {
					key: "leaveStyles",
					value: function(e, t, a, n, s) {
						return {
							height: spring(0, c),
							opacity: spring(0, c),
							top: spring(-100),
							data: t.data
						}
					}
				}, {
					key: "selectItem",
					value: function(e, t, a) {
						return e.preventDefault(), e.stopPropagation(), App.events.emit(this.props.on_select_event_name, {
							index: t
						}), !1
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: classNames(this.props.className, "dropdown", {}),
							onMouseDown: App.doNothing,
							onTouchStart: this.showDropdown,
							onClick: this.showDropdown,
							onTouchEnd: App.doNothing
						}, React.createElement("div", {
							className: "dropdown-display"
						}, this.props.children), React.createElement(TransitionMotion, {
							willEnter: this.enterStyles,
							styles: this.styles(),
							willLeave: this.leaveStyles
						}, this.renderDropdownListUsingStyles))
					}
				}, {
					key: "renderDropdownListUsingStyles",
					value: function(e) {
						var t = this;
						return React.createElement("div", {
							className: classNames({
								"dropdown-list": !0,
								active: this.state.is_dropdown_menu_visible
							})
						}, _.map(e, function(a, n) {
							var s = e[n];
							return t.createDropdownItem(a, n, s)
						}))
					}
				}, {
					key: "createDropdownItem",
					value: function(e, t, n) {
						var s = this,
							i = a(n.data, []),
							r = a(n, ["data"]);
						return React.createElement("div", {
							key: t,
							style: r,
							className: "dropdown-item",
							onTouchStart: function(e) {
								s.selectItem(e, t, i)
							},
							onClick: function(e) {
								s.selectItem(e, t, i)
							}
						}, React.createElement("em", {
							className: classNames("fa", i.is_active ? "fa-dot-circle-o" : "fa-circle-o")
						}), React.createElement("span", null, i.text))
					}
				}]), t
			}(React.Component);
		t["default"] = l
	}, function(t, a, n) {
		"use strict";

		function s(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function i(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function r(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function o(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(a, "__esModule", {
			value: !0
		});
		var c = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			u = n(33),
			d = s(u),
			p = function(t) {
				function a(e, t) {
					i(this, a);
					var n = r(this, Object.getPrototypeOf(a).call(this, e, t)),
						s = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(s, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						hentai_franchise_search_text: "",
						algolia: null,
						throttledPerformSearch: null,
						search_results: null,
						is_loading: !1,
						pending_hentai_franchise_bind: null
					}, n
				}
				return o(a, t), c(a, [{
					key: "componentDidMount",
					value: function() {
						var e = this;
						this.setupEventHandling(), this.setState({
							algolia: algoliasearch(this.props.env.algolia_search_application_id, this.props.env.algolia_search_search_only_api_key),
							throttledPerformSearch: _.throttle(function(t) {
								e.performSearch(t)
							}, 200, {
								trailing: !0
							}),
							search_text: ""
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						App.events.addListener("SEARCH_HENTAI_FRANCHISE", function(t) {
							e.setState({
								hentai_franchise_search_text: t.name
							}, function() {
								e.performSearch(t.name)
							})
						}), App.events.addListener("HENTAI_FRANCHISE_SELECTED", function(t) {
							e.setState({
								pending_hentai_franchise_bind: t.hentai_franchise
							})
						})
					}
				}, {
					key: "render",
					value: function() {
						return d["default"].apply(this)
					}
				}, {
					key: "getIndexName",
					value: function() {
						return "HentaiFranchise"
					}
				}, {
					key: "updateHentaiFranchiseSearchText",
					value: function(e) {
						var t = e.target.value;
						this.setState({
							hentai_franchise_search_text: t
						}), this.state.throttledPerformSearch(t)
					}
				}, {
					key: "onEnter",
					value: function(e, t) {
						13 == e.which && ($(e.target).blur(), t())
					}
				}, {
					key: "performSearch",
					value: function(e) {
						var t = this,
							a = this.getIndexName(),
							n = this.state.algolia.initIndex(a);
						n.search(e, {
							hitsPerPage: 10,
							page: 0,
							facets: "*"
						}, function(e, a) {
							t.searchCallback(e, a)
						})
					}
				}, {
					key: "searchCallback",
					value: function(t, a) {
						return t ? e(t.message) : void this.setState({
							search_results: a.hits
						})
					}
				}, {
					key: "createHentaiFranchise",
					value: function(t) {
						var a = this;
						if (!this.state.is_loading) {
							this.setState({
								is_loading: !0
							});
							var n = {
								hentai_franchise: {
									name: this.state.hentai_franchise_search_text
								}
							};
							console.log("sending..."), $.ajax({
								type: "POST",
								url: "/api/v2/hentai_franchises",
								data: n,
								headers: {
									"X-Directive": "api"
								},
								success: function(e) {
									console.log("success:", e), a.setState({
										is_loading: !1,
										search_results: [e]
									})
								},
								error: function(t) {
									a.setState({
										is_loading: !1
									}), e(t)
								}
							})
						}
					}
				}, {
					key: "searchResultDelete",
					value: function(t, a, n) {
						var s = this;
						this.state.is_loading || (this.setState({
							is_loading: !0
						}), l("delete " + a.title), $.ajax({
							type: "DELETE",
							url: "/api/v2/hentai_franchises/" + a.id,
							headers: {
								"X-Directive": "api"
							},
							success: function(e) {
								l("success:", e), s.setState({
									is_loading: !1
								});
								var t = _.clone(s.state.search_results);
								t.splice(n, 1), s.setState({
									search_results: t
								})
							},
							error: function(t) {
								s.setState({
									is_loading: !1
								}), e(t)
							}
						}))
					}
				}]), a
			}(React.Component);
		a["default"] = p
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						options: i.props.options
					}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "onSelectOptionChange",
					value: function(e, t, a) {
						var n = this;
						e.preventDefault(), e.stopPropagation();
						var s = _.clone(this.state.options);
						return s[t].is_active = !s[t].is_active, this.setState({
							options: s
						}, function() {
							App.events.emit(n.props.on_change_event_name, {
								items: n.state.options
							})
						}), !1
					}
				}, {
					key: "selectAll",
					value: function(e) {
						var t = this;
						e.preventDefault(), e.stopPropagation();
						var a = _.clone(this.state.options);
						return _.each(a, function(e) {
							e.is_active = !1
						}), this.setState({
							options: a
						}, function() {
							App.events.emit(t.props.on_change_event_name, {
								items: t.state.options
							})
						}), !1
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: classNames(this.props.className, "htv-select-multiple", {
								inverse: this.props.is_inverse,
								"tse-scrollable": !this.props.is_display_all
							})
						}, React.createElement("div", {
							className: "tse-content"
						}, React.createElement("div", {
							className: classNames("option", {
								active: 0 == _.filter(this.state.options, {
									is_active: !0
								}).length
							}),
							onClick: this.selectAll
						}, React.createElement("em", {
							className: classNames("fa", 0 == _.filter(this.state.options, {
								is_active: !0
							}).length ? this.props.is_inverse ? "fa-check" : "fa-check-square-o" : this.props.is_inverse ? "fa-square-o hidden" : "fa-square-o")
						}), React.createElement("span", null, "All")), _.map(this.state.options, function(t, a) {
							return React.createElement("div", {
								className: classNames("option", {
									active: t.is_active
								}),
								key: a,
								onClick: function(n) {
									e.onSelectOptionChange(n, a, t)
								}
							}, React.createElement("em", {
								className: classNames("fa", t.is_active ? e.props.is_inverse ? "fa-check" : "fa-check-square-o" : e.props.is_inverse ? "fa-square-o hidden" : "fa-square-o")
							}), React.createElement("span", null, t.text))
						})))
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}

		function s(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function i(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function r(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var o = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			c = a(29),
			l = n(c),
			u = a(30),
			d = n(u),
			p = function(e) {
				function t(e, a) {
					s(this, t);
					var n = i(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(n.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, n), n.props = e, n.state = {
						is_h264_supported: !1,
						is_webm_supported: !1,
						is_ios: !1,
						is_video_player_active: !1,
						is_controls_active: !1,
						controls_timer: null,
						is_fullscreen_supported: !1,
						video_container: null,
						video_dom: null,
						is_playing: !1,
						currentTime: 0,
						is_in_fullscreen_mode: !1,
						progress_style: {},
						scrubber_progress_style: {},
						controls_timeout: 4e3,
						dragging: !1,
						time_progress_style: {},
						time_progress: "",
						time_remaining: "",
						config_dropdown_items: [],
						is_autoplay_on_load: !1,
						default_transcode: {},
						storyboard_frame_style: {}
					}, n
				}
				return r(t, e), o(t, [{
					key: "componentDidMount",
					value: function() {
						var e = this;
						this.setupEventHandling();
						var t = setTimeout(this.deactiveControls, this.state.controls_timeout),
							a = document.querySelector("#video_element"),
							n = App.isIOS();
						this.setState({
							is_h264_supported: !!Modernizr.video.h264,
							is_webm_supported: !!Modernizr.video.webm,
							config_dropdown_items: this.configDropdownItems(),
							is_ios: n,
							controls_timer: t,
							is_fullscreen_supported: this.isFullscreenSupported(),
							video_container: document.querySelector("#video_container"),
							video_dom: a
						}, function() {
							var t = e.getDefaultTranscode();
							e.setState({
								default_transcode: t
							}, function() {
								App.events.emit("htv-video-player-change-resolution", {
									height: t.height,
									url: t.cached_itag_url,
									autoplay: !1
								}), App.events.emit("HTV_VIDEO_PLAYER_REPORTING", {
									is_h264_supported: e.state.is_h264_supported ? "yes" : "no",
									is_webm_supported: e.state.is_webm_supported ? "yes" : "no"
								})
							})
						}), $(document).on("fullscreenchange webkitfullscreenchange mozfullscreenchange MSFullscreenChange", this.onFullscreenChange), $(window).on("resize", _.debounce(this.onScreenResize, 300, {
							leading: !0,
							trailing: !0
						})), window.addEventListener("orientationchange", this.onOrientationChange, !1);
						var s = document.querySelector("#progress_bar_container");
						s.addEventListener("mouseenter", this.progressBarMouseEnter), s.addEventListener("mousedown", this.beginDrag), s.addEventListener("touchstart", this.beginTouchDrag), s.addEventListener("touchmove", this.touchDrag), s.addEventListener("touchend", this.endTouchDrag), s.addEventListener("mousemove", this.drag), s.addEventListener("mouseup", this.endDrag), s.addEventListener("mouseleave", this.progressBarMouseLeave), a.addEventListener("loadedmetadata", function(t) {
							e.state.currentTime > 0 && (e.state.video_dom.currentTime = e.state.currentTime), e.state.is_autoplay_on_load && e.state.video_dom.play()
						}, !1), a.addEventListener("play", function() {
							e.setState({
								is_playing: !0
							})
						}, !1), a.addEventListener("pause", function() {
							e.setState({
								is_playing: !1
							})
						}, !1), a.addEventListener("timeupdate", _.throttle(this.updateProgressBarData, 1e3, {
							leading: !0,
							trailing: !0
						}), !1), a.addEventListener("error", this.onError, !1), document.addEventListener("keydown", this.onKeyDown, !1)
					}
				}, {
					key: "setupEventHandling",
					value: function() {
						var e = this;
						App.events.addListener("HTV_VIDEO_PLAYER_RELOAD", function(t) {
							e.activateVideo();
							var a = Cookies.get("video.height"),
								n = e.state.video_dom.currentSrc;
							n += n.indexOf("?") > -1 ? "&cache_bust=" + (new Date).getTime() : "?cache_bust=" + (new Date).getTime(), e.changeResolution(a, n)
						}), App.events.addListener("htv-video-player-activate", function(t) {
							e.activateVideo()
						}), App.events.addListener("htv-video-player-deactivate", function(t) {
							e.deactivateVideo()
						}), App.events.addListener("htv-video-player-activate-controls", function(t) {
							e.activateControls()
						}), App.events.addListener("htv-video-player-change-resolution", function(t) {
							e.changeResolution(t.height, t.url, t.autoplay)
						})
					}
				}, {
					key: "getDefaultTranscode",
					value: function() {
						var e = Cookies.get("video.height"),
							t = _.filter(this.state.config_dropdown_items, {
								height: e
							});
						return 0 == t.length ? this.state.config_dropdown_items[0] : t[0]
					}
				}, {
					key: "generateStyleForFrame",
					value: function(e, t, a) {
						var n = t.num_horizontal_frames * t.num_vertical_frames,
							s = parseInt(Math.floor(e / n)),
							i = a[s],
							r = e % n,
							o = r % t.num_horizontal_frames,
							c = parseInt(r / t.num_horizontal_frames),
							l = o * t.frame_width,
							u = c * t.frame_height;
						return {
							width: t.frame_width + "px",
							height: t.frame_height + "px",
							background: "url('" + i.url + "') no-repeat",
							backgroundPosition: -l + "px " + -u + "px"
						}
					}
				}, {
					key: "updateStoryboardFrame",
					value: function(e, t, a) {
						if (!this.props.hentai_video_storyboards || 0 == this.props.hentai_video_storyboards.length) return void(a && a());
						var n = $("#progress_bar_container"),
							s = n.width(),
							i = e.offsetX;
						if (t) {
							var r = e.changedTouches[0];
							i = parseInt(r.clientX) - n.offset().left
						}
						var o = Math.min(i / s, 1),
							c = this.props.hentai_video_storyboards[0],
							l = parseInt(Math.floor(o * c.num_total_frames)),
							u = this.generateStyleForFrame(l, c, this.props.hentai_video_storyboards);
						u.left = s * o, this.setState({
							storyboard_frame_style: u
						}, function() {
							a && a()
						})
					}
				}, {
					key: "updateDragData",
					value: function(e, t, a, n) {
						var s = $("#progress_bar_container"),
							i = s.width(),
							r = e.offsetX;
						if (a) {
							var o = e.changedTouches[0];
							r = parseInt(o.clientX) - s.offset().left
						}
						var c = Math.min(r / i, 1),
							l = 100 * c;
						this.setState({
							dragging: t,
							scrubber_progress_style: {
								width: l + "%"
							},
							time_progress_style: {
								left: r
							},
							time_progress: App.secondsToHuman(c * this.state.video_dom.duration)
						}, function() {
							n && n()
						})
					}
				}, {
					key: "progressBarMouseEnter",
					value: function(e) {
						e.preventDefault(), e.stopPropagation(), this.setState({
							is_storyboard_frame_visible: !0
						})
					}
				}, {
					key: "beginDrag",
					value: function(e) {
						e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !0, !1)
					}
				}, {
					key: "beginTouchDrag",
					value: function(e) {
						var t = this;
						e.preventDefault(), e.stopPropagation(), this.setState({
							is_storyboard_frame_visible: !0
						}, function() {
							t.updateDragData(e, !0, !0)
						})
					}
				}, {
					key: "drag",
					value: function(e) {
						var t = this;
						e.preventDefault(), e.stopPropagation(), this.activateControls(function() {
							t.updateStoryboardFrame(e, !1, function() {
								t.state.dragging && t.updateDragData(e, !0, !1)
							})
						})
					}
				}, {
					key: "touchDrag",
					value: function(e) {
						var t = this;
						e.preventDefault(), e.stopPropagation(), this.activateControls(function() {
							t.updateStoryboardFrame(e, !0, function() {
								t.state.dragging && t.updateDragData(e, !0, !0)
							})
						})
					}
				}, {
					key: "endDrag",
					value: function(e) {
						var t = this;
						e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !1, !1, function() {
							t.seekTo(e)
						})
					}
				}, {
					key: "endTouchDrag",
					value: function(e) {
						var t = this;
						e.preventDefault(), e.stopPropagation(), this.setState({
							is_storyboard_frame_visible: !1
						}, function() {
							t.updateDragData(e, !1, !0, function() {
								t.touchSeekTo(e)
							})
						})
					}
				}, {
					key: "progressBarMouseLeave",
					value: function(e) {
						e.preventDefault(), e.stopPropagation(), this.setState({
							dragging: !1,
							is_storyboard_frame_visible: !1
						})
					}
				}, {
					key: "seekTo",
					value: function(e) {
						e.preventDefault(), e.stopPropagation();
						var t = $("#progress_bar_container").width(),
							a = e.offsetX / t;
						a > 1 && (a = 1), this.state.video_dom.currentTime = this.state.video_dom.duration * a, this.updateProgressBarData(), this.activateControls(), this.state.video_dom.paused && this.togglePlay(e)
					}
				}, {
					key: "touchSeekTo",
					value: function(e) {
						e.preventDefault(), e.stopPropagation();
						var t = $("#progress_bar_container"),
							a = t.width(),
							n = e.changedTouches[0],
							s = parseInt(n.clientX) - t.offset().left,
							i = s / a;
						i > 1 && (i = 1), this.state.video_dom.currentTime = this.state.video_dom.duration * i, this.updateProgressBarData(), this.activateControls(), this.state.video_dom.paused && this.togglePlay(e)
					}
				}, {
					key: "isFullscreenSupported",
					value: function() {
						var e = !!(document.fullscreenEnabled || document.webkitFullscreenEnabled || document.mozFullScreenEnabled || document.msFullscreenEnabled);
						return e || this.state.is_ios || App.isIOS()
					}
				}, {
					key: "onFullscreenChange",
					value: function(e) {
						this.refitVideo()
					}
				}, {
					key: "onScreenResize",
					value: function(e) {
						this.refitVideo()
					}
				}, {
					key: "onOrientationChange",
					value: function(e) {
						this.refitVideo()
					}
				}, {
					key: "refitVideo",
					value: function() {
						var e = ($(window).width(), $(window).height()),
							t = this.state.video_dom.videoWidth,
							a = this.state.video_dom.videoHeight,
							n = t / a,
							s = n * e;
						$(".player-container").css({
							width: s + "px"
						})
					}
				}, {
					key: "emitDeactivateVideo",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), App.events.emit("htv-video-player-deactivate", {}), !1
					}
				}, {
					key: "activateVideo",
					value: function() {
						this.state.video_dom.play(), this.refitVideo(), this.setState({
							is_video_player_active: !0
						}), this.activateControls()
					}
				}, {
					key: "deactivateVideo",
					value: function() {
						this.state.video_dom.pause(), this.setState({
							is_video_player_active: !1
						})
					}
				}, {
					key: "doNothing",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), !1
					}
				}, {
					key: "handleMainPaneClick",
					value: function(e) {
						e.preventDefault(), e.stopPropagation(), this.state.is_controls_active && this.togglePlay(e), this.activateControls()
					}
				}, {
					key: "activateControls",
					value: function(e) {
						clearTimeout(this.state.controls_timer);
						var t = setTimeout(this.deactiveControls, this.state.controls_timeout);
						this.setState({
							is_controls_active: !0,
							controls_timer: t
						}, function() {
							e && "function" == typeof e && e()
						})
					}
				}, {
					key: "deactiveControls",
					value: function() {
						this.setState({
							is_controls_active: !1
						})
					}
				}, {
					key: "isInFullscreenMode",
					value: function() {
						return document.fullscreenElement || document.webkitFullscreenElement || document.mozFullScreenElement || document.msFullscreenElement
					}
				}, {
					key: "activateFullscreen",
					value: function() {
						this.state.is_ios ? this.state.video_dom.webkitEnterFullscreen() : this.state.video_container.requestFullscreen ? this.state.video_container.requestFullscreen() : this.state.video_container.webkitRequestFullscreen ? this.state.video_container.webkitRequestFullscreen() : this.state.video_container.mozRequestFullScreen ? this.state.video_container.mozRequestFullScreen() : this.state.video_container.msRequestFullscreen && this.state.video_container.msRequestFullscreen(), this.setState({
							is_in_fullscreen_mode: !0
						})
					}
				}, {
					key: "deactivateFullscreen",
					value: function() {
						document.exitFullscreen ? document.exitFullscreen() : document.webkitExitFullscreen ? document.webkitExitFullscreen() : document.mozCancelFullScreen ? document.mozCancelFullScreen() : document.msExitFullscreen && document.msExitFullscreen(), this.setState({
							is_in_fullscreen_mode: !1
						})
					}
				}, {
					key: "toggleFullscreen",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.isInFullscreenMode() ? this.deactivateFullscreen() : this.activateFullscreen(), !1
					}
				}, {
					key: "togglePlay",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.state.video_dom.paused ? (this.state.video_dom.play(), this.setState({
							is_playing: !0
						})) : (this.state.video_dom.pause(), this.setState({
							is_playing: !1
						})), this.activateControls(), !1
					}
				}, {
					key: "updateProgressBarData",
					value: function() {
						var e = this,
							t = this.state.video_dom.currentTime || 0,
							a = this.state.video_dom.duration || 0,
							n = "0%",
							s = 0;
						0 != a && (s = t / a || 0, n = 100 * s + "%"), this.setState({
							currentTime: t,
							progress_style: {
								width: n
							}
						}, function() {
							if (!e.state.dragging) {
								var i = s * $("#progress_bar_container").width();
								e.setState({
									scrubber_progress_style: {
										width: n
									},
									time_progress_style: {
										left: i
									},
									time_progress: App.secondsToHuman(t),
									time_remaining: App.secondsToHuman(a - t)
								})
							}
						})
					}
				}, {
					key: "onError",
					value: function(e) {
						var t = this.state.video_dom.error.code,
							a = null;
						switch (t) {
							case MediaError.MEDIA_ERR_ABORTED:
								a = "You aborted the video playback.";
								break;
							case MediaError.MEDIA_ERR_NETWORK:
								a = "A network error occurred.  Refresh the page to fix it.";
								break;
							case MediaError.MEDIA_ERR_DECODE:
								a = "Video decoding problem occurred.  Refresh the page to try to fix it, or use a modern browser like Google Chrome.";
								break;
							case MediaError.MEDIA_ERR_SRC_NOT_SUPPORTED:
								a = "Your network died while loading the video or your browser is too shitty to play videos.  Refresh the page to fix problem, or use a modern browser like Google Chrome.";
								break;
							default:
								a = "An unknown error occurred."
						}
						var n = this.state.video_dom.getAttribute("src");
						App.events.emit("HTV_VIDEO_PLAYER_REPORTING", {
							video_player_msg: "ERROR_CODE: " + this.state.video_dom.error.code + " | MSG: " + a + " | TRANSCODE_URL: " + n + " | TIMESTAMP: " + e.timeStamp
						}), App.events.emit("HTV_VIDEO_PLAYER_ERROR", {
							msg: a,
							is_h264_supported: this.state.is_h264_supported,
							is_webm_supported: this.state.is_webm_supported,
							transcode_url: n
						})
					}
				}, {
					key: "configDropdownItems",
					value: function() {
						var e = !!Modernizr.video.h264,
							t = !!Modernizr.video.webm;
						return _.filter(this.props.transcodes, function(a) {
							return "video/mp4" == a.video_type ? e : "video/webm" == a.video_type ? e ? !1 : t : !1
						})
					}
				}, {
					key: "changeResolution",
					value: function(e, t) {
						var a = arguments.length <= 2 || void 0 === arguments[2] ? !0 : arguments[2],
							n = this.state.video_dom;
						if (n.currentSrc != t) {
							n.pause();
							var s = n.currentTime;
							n.setAttribute("src", t), n.load(), a && Cookies.set("video.height", e, {
								domain: "." + window.location.hostname,
								expires: 15552e3
							}), this.setState({
								is_autoplay_on_load: a,
								currentTime: s
							}), this.activateControls()
						}
					}
				}, {
					key: "onKeyDown",
					value: function(e) {
						this.state.is_video_player_active && (32 == e.keyCode ? this.togglePlay(e) : 27 == e.keyCode && this.emitDeactivateVideo(e))
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							id: "video_container",
							className: classNames("htv-video-player", {
								active: this.state.is_video_player_active
							}),
							onMouseMove: this.activateControls,
							onMouseDown: this.handleMainPaneClick,
							onTouchStart: this.handleMainPaneClick,
							onClick: this.doNothing,
							onTouchEnd: this.doNothing
						}, React.createElement("div", {
							className: "player-container flex-col justify-center"
						}, React.createElement("video", {
							id: "video_element",
							preload: "auto",
							src: ""
						}), React.createElement("div", {
							className: classNames("video-paused-overlay", {
								paused: !this.state.is_playing
							})
						}), React.createElement("div", {
							className: classNames("giant-resume-icon", {
								active: !this.state.is_playing
							})
						}, React.createElement("em", {
							className: "fa fa-play"
						})), React.createElement("div", {
							className: classNames("player-controls top-bar", {
								active: this.state.is_controls_active
							})
						}, React.createElement("div", {
							className: "close-icon",
							onMouseDown: this.emitDeactivateVideo,
							onTouchStart: this.emitDeactivateVideo,
							onClick: this.deactivateFullscreen,
							onTouchEnd: this.deactivateFullscreen
						}, React.createElement("span", null, "×")), React.createElement("div", {
							className: "flex"
						}), this.state.is_ios ? null : React.createElement(d["default"], {
							className: "",
							video: this.state.video_dom
						}), this.state.config_dropdown_items.length > 1 ? React.createElement(l["default"], {
							className: "config-icon",
							dropdown_items: this.state.config_dropdown_items
						}) : null), React.createElement("div", {
							className: classNames("player-controls bottom-bar", {
								active: this.state.is_controls_active
							})
						}, React.createElement("div", {
							className: "play-pause-icon",
							onMouseDown: this.togglePlay,
							onTouchStart: this.togglePlay,
							onClick: this.doNothing,
							onTouchEnd: this.doNothing
						}, React.createElement("em", {
							className: classNames("fa", {
								"fa-play": !this.state.is_playing,
								"fa-pause": this.state.is_playing
							})
						})), React.createElement("div", {
							className: classNames("storyboard-frame", {
								active: this.state.is_storyboard_frame_visible
							}),
							style: this.state.storyboard_frame_style
						}), React.createElement("div", {
							id: "progress_bar_container",
							className: "progress-bar-container flex"
						}, React.createElement("div", {
							className: "progress-bar"
						}, React.createElement("div", {
							className: "progress",
							style: this.state.progress_style
						})), React.createElement("div", {
							className: "scrubber-progress",
							style: this.state.scrubber_progress_style
						})), React.createElement("div", {
							className: "time-progress",
							style: this.state.time_progress_style
						}, this.state.time_progress), React.createElement("div", {
							className: "time-remaining"
						}, this.state.time_remaining), React.createElement("div", {
							className: classNames("fullscreen-icon", {
								supported: this.state.is_fullscreen_supported
							}),
							onMouseDown: this.doNothing,
							onTouchStart: this.doNothing,
							onClick: this.toggleFullscreen,
							onTouchEnd: this.toggleFullscreen
						}, React.createElement("em", {
							className: classNames("fa", {
								"fa-expand": !this.state.is_in_fullscreen_mode,
								"fa-compress": this.state.is_in_fullscreen_mode
							})
						})))))
					}
				}]), t
			}(React.Component);
		t["default"] = p
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			var a = {};
			for (var n in e) t.indexOf(n) >= 0 || Object.prototype.hasOwnProperty.call(e, n) && (a[n] = e[n]);
			return a
		}

		function n(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function s(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function i(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var r = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			o = [750, 19],
			c = [600, 25],
			l = function(e) {
				function t(e, a) {
					n(this, t);
					var i = s(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						is_dropdown_menu_visible: !1,
						current_selected_height: 720
					}, i
				}
				return i(t, e), r(t, [{
					key: "componentDidMount",
					value: function() {
						var e = this;
						this.setupEventHandling(), App.events.addListener("htv-video-player-change-resolution", function(t) {
							e.changeResolution(t.height, t.url, t.autoplay)
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "showDropdown",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.setState({
							is_dropdown_menu_visible: !0
						}), document.addEventListener("click", this.hideDropdown), document.addEventListener("touchstart", this.hideDropdown), !1
					}
				}, {
					key: "hideDropdown",
					value: function() {
						this.setState({
							is_dropdown_menu_visible: !1
						}), document.removeEventListener("click", this.hideDropdown), document.removeEventListener("touchstart", this.hideDropdown)
					}
				}, {
					key: "enterStyles",
					value: function(e, t, a, n, s) {
						return {
							height: 0,
							opacity: 1,
							top: 0,
							data: this.props.dropdown_items[e]
						}
					}
				}, {
					key: "styles",
					value: function() {
						if (!this.state.is_dropdown_menu_visible) return {};
						var e = this.props.dropdown_items;
						return Object.keys(e).reduce(function(t, a) {
							return t[a] = {
								height: spring(42, o),
								opacity: spring(1, o),
								top: 0,
								data: e[a]
							}, t
						}, {})
					}
				}, {
					key: "leaveStyles",
					value: function(e, t, a, n, s) {
						return {
							height: spring(0, c),
							opacity: spring(0, c),
							top: spring(-100),
							data: t.data
						}
					}
				}, {
					key: "doNothing",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), !1
					}
				}, {
					key: "emitChangeResolution",
					value: function(e, t) {
						App.events.emit("htv-video-player-change-resolution", {
							height: e,
							url: t,
							autoplay: !0
						})
					}
				}, {
					key: "changeResolution",
					value: function(e, t) {
						this.state.current_selected_height != e && this.setState({
							current_selected_height: e
						})
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: classNames(this.props.className, "dropdown icon-only right-margin", {}),
							onMouseDown: this.doNothing,
							onTouchStart: this.showDropdown,
							onClick: this.showDropdown,
							onTouchEnd: this.doNothing
						}, React.createElement("div", {
							className: "dropdown-display"
						}, React.createElement("em", {
							className: "fa fa-ellipsis-v"
						})), React.createElement(TransitionMotion, {
							willEnter: this.enterStyles,
							styles: this.styles(),
							willLeave: this.leaveStyles
						}, this.renderDropdownListUsingStyles))
					}
				}, {
					key: "renderDropdownListUsingStyles",
					value: function(e) {
						var t = this;
						return React.createElement("div", {
							className: classNames({
								"dropdown-list": !0,
								active: this.state.is_dropdown_menu_visible
							})
						}, _.map(e, function(a, n) {
							var s = e[n];
							return t.createDropdownItem(a, n, s)
						}))
					}
				}, {
					key: "createDropdownItem",
					value: function(e, t, n) {
						var s = this,
							i = a(n.data, []),
							r = a(n, ["data"]);
						return React.createElement("div", {
							key: t,
							style: r,
							className: "dropdown-item",
							onTouchStart: function(e) {
								s.emitChangeResolution(i.height, i.cached_itag_url)
							},
							onClick: function(e) {
								s.emitChangeResolution(i.height, i.cached_itag_url)
							}
						}, React.createElement("em", {
							className: classNames("fa", this.state.current_selected_height == i.height ? "fa-dot-circle-o" : "fa-circle-o")
						}), React.createElement("span", null, i.height, "P"))
					}
				}]), t
			}(React.Component);
		t["default"] = l
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						volume: 1,
						volume_style: {},
						dragging: !1,
						jquery_volume_bar_container: null
					}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						var e = this;
						this.setupEventHandling();
						var t = document.querySelector("#volume_bar_container");
						t.addEventListener("mousedown", this.beginDrag, !1), t.addEventListener("touchstart", this.beginTouchDrag, !1), t.addEventListener("touchmove", this.touchDrag, !1), t.addEventListener("touchend", this.endTouchDrag, !1), t.addEventListener("mousemove", this.drag, !1), t.addEventListener("mouseup", this.endDrag, !1), t.addEventListener("mouseleave", this.volumeBarMouseLeave, !1), this.setState({
							jquery_volume_bar_container: $(t)
						}, function() {
							var t = Cookies.get("video.volume") || 1;
							e.setVolume(t)
						})
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "updateDragData",
					value: function(e, t, a) {
						var n = this,
							s = this.state.jquery_volume_bar_container,
							i = s.width(),
							r = e.offsetX;
						if (a) {
							var o = e.changedTouches[0];
							r = parseInt(o.clientX) - s.offset().left
						}
						var c = Math.min(r / i, 1),
							l = c;
						this.setState({
							dragging: t
						}, function() {
							n.setVolume(l)
						})
					}
				}, {
					key: "beginDrag",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !0, !1), !1
					}
				}, {
					key: "beginTouchDrag",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !0, !0), !1
					}
				}, {
					key: "drag",
					value: function(e) {
						return this.state.dragging ? (e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !0, !1), App.events.emit("htv-video-player-activate-controls"), !1) : void 0
					}
				}, {
					key: "touchDrag",
					value: function(e) {
						return this.state.dragging ? (e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !0, !0), App.events.emit("htv-video-player-activate-controls"), !1) : void 0
					}
				}, {
					key: "endDrag",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !1, !1), !1
					}
				}, {
					key: "endTouchDrag",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.updateDragData(e, !0, !0), !1
					}
				}, {
					key: "volumeBarMouseLeave",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.setState({
							dragging: !1
						}), !1
					}
				}, {
					key: "setVolume",
					value: function(e) {
						var t = this,
							a = parseFloat(e);
						0 > a ? a = 0 : a > 1 && (a = 1), this.setState({
							volume: a,
							volume_style: {
								width: 100 * a + "%"
							}
						}, function() {
							Cookies.set("video.volume", a, {
								domain: ".hanime.tv",
								expires: 15552e3
							}), t.props.video.volume = a
						})
					}
				}, {
					key: "volumeChange",
					value: function(e, t) {
						e.preventDefault(), e.stopPropagation();
						var a = parseFloat(this.state.volume) + t;
						return 0 > a ? a = 0 : a > 1 && (a = 1), this.setVolume(a), !1
					}
				}, {
					key: "render",
					value: function() {
						var e = this;
						return React.createElement("div", {
							className: "htv-video-player-volume-control",
							onTouchStart: App.doNothing,
							onMouseDown: App.doNothing,
							onClick: App.doNothing,
							onTouchEnd: App.doNothing
						}, React.createElement("div", {
							className: "volume volume-down",
							onTouchStart: function(t) {
								e.volumeChange(t, -.05)
							},
							onMouseDown: App.doNothing,
							onClick: function(t) {
								e.volumeChange(t, -.05)
							},
							onTouchEnd: App.doNothing
						}, React.createElement("em", {
							className: "fa fa-minus"
						})), React.createElement("div", {
							id: "volume_bar_container",
							className: "volume-bar-container flex"
						}, React.createElement("div", {
							className: "volume-bar"
						}, React.createElement("div", {
							className: "volume",
							style: this.state.volume_style
						}))), React.createElement("div", {
							className: "volume volume-up",
							onTouchStart: function(t) {
								e.volumeChange(t, .05)
							},
							onMouseDown: App.doNothing,
							onClick: function(t) {
								e.volumeChange(t, .05)
							},
							onTouchEnd: App.doNothing
						}, React.createElement("em", {
							className: "fa fa-plus"
						})))
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function n(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var i = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			r = function(e) {
				function t(e, s) {
					a(this, t);
					var i = n(this, Object.getPrototypeOf(t).call(this, e, s)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						is_disabled_by_user_click_close: !1
					}, i
				}
				return s(t, e), i(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "componentWillUnmount",
					value: function() {}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "closeSmartBanner",
					value: function() {
						this.setState({
							is_disabled_by_user_click_close: !0
						})
					}
				}, {
					key: "isScrollTopWithinRange",
					value: function() {
						return this.props.scroll_top ? this.props.scroll_top < this.props.scroll_top_start ? !1 : !(this.props.scroll_top > this.props.scroll_top_end) : !1
					}
				}, {
					key: "isBannerCorrectSize",
					value: function() {
						return this.props.viewport_width < 481 && "mobile" == this.props.size ? !0 : this.props.viewport_width < 951 && "tablet" == this.props.size ? !0 : this.props.viewport_width >= 951 && "desktop" == this.props.size
					}
				}, {
					key: "isBannerActive",
					value: function() {
						return this.isScrollTopWithinRange() && !this.state.is_disabled_by_user_click_close && this.isBannerCorrectSize()
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement(ReactCSSTransitionGroup, {
							transitionName: "smart-banner",
							transitionAppear: !0,
							transitionAppearTimeout: 500,
							transitionEnterTimeout: 500,
							transitionLeaveTimeout: 500
						}, this.isBannerActive() ? React.createElement("div", {
							key: 1,
							className: classNames(this.props.className, "smart-banner-content")
						}, React.createElement("div", {
							className: "ie-placement-fixer"
						}, this.props.children), React.createElement("div", {
							className: "close flex-row justify-center align-center growing-icon transition-all",
							title: "Close Banner",
							onClick: this.closeSmartBanner
						}, React.createElement("em", {
							className: "fa fa-close"
						}))) : null)
					}
				}]), t
			}(React.Component);
		t["default"] = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			var a = {};
			for (var n in e) t.indexOf(n) >= 0 || Object.prototype.hasOwnProperty.call(e, n) && (a[n] = e[n]);
			return a
		}

		function n(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function s(e, t) {
			if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
			return !t || "object" != typeof t && "function" != typeof t ? e : t
		}

		function i(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		var r = function() {
				function e(e, t) {
					for (var a = 0; a < t.length; a++) {
						var n = t[a];
						n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
					}
				}
				return function(t, a, n) {
					return a && e(t.prototype, a), n && e(t, n), t
				}
			}(),
			o = [750, 19],
			c = [600, 25],
			l = function(e) {
				function t(e, a) {
					n(this, t);
					var i = s(this, Object.getPrototypeOf(t).call(this, e, a)),
						r = ["constructor", "render"];
					return Object.getOwnPropertyNames(i.constructor.prototype).forEach(function(e) {
						_.includes(r, e) || "function" != typeof this[e] || (this[e] = this[e].bind(this))
					}, i), i.props = e, i.state = {
						is_dropdown_menu_visible: !1
					}, i
				}
				return i(t, e), r(t, [{
					key: "componentDidMount",
					value: function() {
						this.setupEventHandling()
					}
				}, {
					key: "setupEventHandling",
					value: function() {}
				}, {
					key: "showDropdown",
					value: function(e) {
						return e.preventDefault(), e.stopPropagation(), this.setState({
							is_dropdown_menu_visible: !0
						}), document.addEventListener("mousedown", this.hideDropdown), document.addEventListener("touchstart", this.hideDropdown), !1
					}
				}, {
					key: "hideDropdown",
					value: function() {
						this.setState({
							is_dropdown_menu_visible: !1
						}), document.removeEventListener("mousedown", this.hideDropdown), document.removeEventListener("touchstart", this.hideDropdown)
					}
				}, {
					key: "enterStyles",
					value: function(e, t, a, n, s) {
						return {
							height: 0,
							opacity: 1,
							top: 0,
							data: this.props.user_dropdown_items[e]
						}
					}
				}, {
					key: "styles",
					value: function() {
						if (!this.state.is_dropdown_menu_visible) return {};
						var e = this.props.user_dropdown_items;
						return Object.keys(e).reduce(function(t, a) {
							return t[a] = {
								height: spring(42, o),
								opacity: spring(1, o),
								top: 0,
								data: e[a]
							}, t
						}, {})
					}
				}, {
					key: "leaveStyles",
					value: function(e, t, a, n, s) {
						return {
							height: spring(0, c),
							opacity: spring(0, c),
							top: spring(-100),
							data: t.data
						}
					}
				}, {
					key: "navigateTo",
					value: function(e, t) {
						return e.preventDefault(), e.stopPropagation(), this.state.is_dropdown_menu_visible ? (window.location.href = t, !1) : void 0
					}
				}, {
					key: "render",
					value: function() {
						return React.createElement("div", {
							className: classNames(this.props.className, {
								dropdown: !0
							})
						}, React.createElement("div", {
							className: "dropdown-display",
							onTouchStart: this.showDropdown,
							onMouseDown: this.showDropdown
						}, React.createElement("div", {
							className: "selected-item"
						}, this.props.current_user.name), React.createElement("em", {
							className: "caret fa fa-ellipsis-v"
						})), React.createElement(TransitionMotion, {
							willEnter: this.enterStyles,
							styles: this.styles(),
							willLeave: this.leaveStyles
						}, this.renderDropdownListUsingStyles))
					}
				}, {
					key: "renderDropdownListUsingStyles",
					value: function(e) {
						var t = this;
						return React.createElement("div", {
							className: classNames({
								"dropdown-list": !0,
								active: this.state.is_dropdown_menu_visible
							})
						}, _.map(e, function(a, n) {
							var s = e[n];
							return t.createDropdownItem(a, n, s)
						}))
					}
				}, {
					key: "createDropdownItem",
					value: function(e, t, n) {
						var s = this,
							i = a(n.data, []),
							r = a(n, ["data"]),
							o = i.type;
						switch (o) {
							case "link":
								return React.createElement("a", {
									className: "dropdown-item",
									key: t,
									style: r,
									href: i.url,
									onTouchStart: function(e) {
										s.navigateTo(e, i.url)
									},
									onMouseDown: function(e) {
										s.navigateTo(e, i.url)
									},
									onClick: App.doNothing
								}, React.createElement("em", {
									className: i.icon_classes
								}), React.createElement("span", null, i.text));
							default:
								return React.createElement("div", {
									key: t,
									style: r,
									className: "dropdown-item",
									onClick: function(e) {
										console.log("doing nothing")
									}
								}, React.createElement("p", null, i.text))
						}
					}
				}]), t
			}(React.Component);
		t["default"] = l
	}, function(e, t) {
		"use strict";
		Object.defineProperty(t, "__esModule", {
			value: !0
		}), t["default"] = function() {
			var e = this;
			return React.createElement("div", {
				className: "htv-franchise-manager container-fluid"
			}, React.createElement("div", {
				className: "row"
			}, React.createElement("div", {
				className: "col-xs-12"
			}, React.createElement("h4", null, "Hentai Franchise Manager"), React.createElement("div", {
				className: "flex-row"
			}, React.createElement("input", {
				type: "text",
				id: "search_input",
				className: "input-text flex",
				placeholder: "Type in a franchise name...",
				onChange: this.updateHentaiFranchiseSearchText,
				onKeyUp: function(t) {
					e.onEnter(t, function() {
						e.performSearch(t.target.value)
					})
				}
			}), React.createElement("div", {
				className: "btn btn-primary",
				onClick: this.createHentaiFranchise
			}, "Create")), this.state.search_results ? React.createElement("p", null, "Number of results: ", this.state.search_results.length) : null, React.createElement("div", {
				className: "flex-col"
			}, _.map(this.state.search_results, function(t, a) {
				return React.createElement("div", {
					className: classNames("search-result flex-row", {
						selected: e.state.pending_hentai_franchise_bind && e.state.pending_hentai_franchise_bind.id == t.id
					}),
					key: t.id
				}, React.createElement("div", {
					className: "hentai-franchise",
					onClick: function(e) {
						App.emit("HENTAI_FRANCHISE_SELECTED", {
							hentai_franchise: t
						})
					}
				}, t.title), React.createElement("span", {
					className: "flex"
				}), React.createElement("div", {
					className: "icon danger-bgcolor-hover",
					onClick: function(n) {
						e.searchResultDelete(n, t, a)
					}
				}, React.createElement("em", {
					className: "fa fa-trash-o"
				})))
			})))))
		}
	}, function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}
		
		Object.defineProperty(t, "__esModule", {
			value: !0
		}), t["default"] = function() {
			var e = this;
			return React.createElement("div", {
				className: "container-fluid admin-dashboard"
			}, React.createElement(i["default"], this.props), React.createElement("div", {
				className: "row"
			}, React.createElement("div", {
				className: "col-xs-2"
			}, React.createElement(o["default"], this.props)), React.createElement("div", {
				className: "col-xs-10 video-manager"
			}, React.createElement("h4", null, "Hentai Video Finder (id or slug)"), React.createElement("div", {
				className: "flex-row"
			}, React.createElement("input", {
				type: "text",
				id: "hv_search_input",
				className: "input-text flex",
				placeholder: "Type in a hentai video id or slug...",
				onKeyUp: function(t) {
					e.onEnter(t, e.findHentaiVideo)
				}
			}), React.createElement("div", {
				className: "btn btn-primary",
				onClick: function(t) {
					e.findHentaiVideo(t)
				}
			}, "Find"), React.createElement("div", {
				className: "btn btn-primary",
				onClick: function(t) {
					e.findNextHentaiVideo(t)
				}
			}, "Next")), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-9 padding-15"
			}, React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-6 flex-row align-center"
			}, React.createElement("strong", null, "[ ", this.state.hentai_video.id ? React.createElement("a", {
				href: "/hentai-videos/" + this.state.hentai_video.slug
			}, this.state.hentai_video.id) : React.createElement("span", {
				className: "danger-color"
			}, " n/a"), " ]"), " ", React.createElement("input", {
				type: "text",
				className: "flex",
				placeholder: "Name",
				value: this.state.hentai_video.name,
				onChange: function(t) {
					e.updateFields(["name", "tag_term"], t.target.value)
				}
			})), React.createElement("section", {
				className: "col-xs-6 flex-row align-center"
			}, React.createElement("strong", null, "slug:"), " ", React.createElement("input", {
				type: "text",
				className: "flex",
				placeholder: "Slug",
				value: this.state.hentai_video.slug,
				onChange: function(t) {
					e.updateField("slug", t.target.value)
				}
			}))), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-12 franchise-info"
			}, React.createElement("p", null, "hentai_franchise_id: ", this.state.hentai_video && this.state.hentai_video.hentai_franchise_id ? React.createElement("strong", null, this.state.hentai_video.hentai_franchise_id) : React.createElement("span", {
				className: "danger-color"
			}, " n/a")), React.createElement("span", null, this.state.pending_hentai_franchise_bind && this.state.pending_hentai_franchise_bind.id != this.state.hentai_video.hentai_franchise_id ? React.createElement("div", {
				className: "btn btn-primary",
				onClick: this.verifyBindHentaiFranchise
			}, "Bind to:", React.createElement("br", null), this.state.pending_hentai_franchise_bind.title) : null), React.createElement(l["default"], this.props))), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-12"
			}, "brand:", React.createElement("select", {
				className: "brand-select",
				defaultValue: this.state.hentai_video.brand,
				onChange: function(t) {
					e.updateField("brand", t.target.value)
				}
			}, _.map(this.props.brands, function(e, t) {
				return React.createElement("option", {
					value: e,
					key: t
				}, e)
			})))), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-12"
			}, "released_at:", React.createElement("input", {
				type: "text",
				className: "flex",
				placeholder: "Release Date",
				value: this.state.hentai_video.released_at,
				onChange: function(t) {
					e.updateField("released_at", t.target.value)
				}
			}))), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-12"
			}, "description:", React.createElement("textarea", {
				className: "description-input",
				value: this.state.hentai_video.description,
				onChange: function(t) {
					e.updateField("description", t.target.value)
				}
			}))), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-6 flex-row align-center"
			}, "is_hard_subtitled: ", React.createElement("div", {
				className: classNames("subtitling success-color", {
					active: this.state.hentai_video.is_hard_subtitled
				}),
				onClick: function(t) {
					e.updateField("is_hard_subtitled", !0)
				}
			}, React.createElement("em", {
				className: classNames("fa", this.state.hentai_video.is_hard_subtitled ? "fa-dot-circle-o" : "fa-circle-thin")
			}), "  yes"), "  ", React.createElement("div", {
				className: classNames("subtitling danger-color", {
					active: !this.state.hentai_video.is_hard_subtitled
				}),
				onClick: function(t) {
					e.updateField("is_hard_subtitled", !1)
				}
			}, React.createElement("em", {
				className: classNames("fa", this.state.hentai_video.is_hard_subtitled ? "fa-circle-thin" : "fa-dot-circle-o")
			}), "  no")), React.createElement("section", {
				className: "col-xs-6 flex-row align-center"
			}, "is_censored: ", React.createElement("div", {
				className: classNames("censorship danger-color", {
					active: this.state.hentai_video.is_censored
				}),
				onClick: function(t) {
					e.updateField("is_censored", !0)
				}
			}, React.createElement("img", {
				src: "https://web.archive.org/web/20170201123401/https://static1.hanime.tv/images/lirik_feels.png",
				width: "40"
			}), "censored"), React.createElement("div", {
				className: classNames("censorship success-color", {
					active: !this.state.hentai_video.is_censored
				}),
				onClick: function(t) {
					e.updateField("is_censored", !1)
				}
			}, React.createElement("img", {
				src: "https://web.archive.org/web/20170201123401/https://static2.hanime.tv/images/soda_c.png",
				width: "40"
			}), "uncensored"))), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-12"
			}, "video_id: ", React.createElement("div", {
				className: "tse-scrollable transcodes-container"
			}, React.createElement("div", {
				className: "tse-content"
			}, _.map(this.state.transcodes, function(t, a) {
				return React.createElement("div", {
					className: classNames("transcode flex-row align-center", {
						active: t.id == e.state.hentai_video.video_id
					}),
					key: a,
					onClick: function(a) {
						e.selectTranscode(a, t)
					}
				}, t.title)
			}))), React.createElement("button", {
				className: classNames("btn btn-primary btn-shadow btn-sm", {
					hidden: this.state.hentai_video.video_id == this.state.cached_hentai_video.video_id || !this.state.hentai_video.id
				}),
				onClick: function(t) {
					e.updateFieldDb("video_id")
				},
				disabled: this.state.is_loading
			}, React.createElement("span", {
				className: "text"
			}, "Update Video ID"))))), React.createElement("section", {
				className: "col-xs-3 padding-15"
			}, React.createElement("p", null, "cover_url:"), React.createElement("div", {
				className: "frame cover-drop"
			}, React.createElement(d["default"], {
				className: "",
				data: this.state.hentai_video,
				is_load_image_immediately: !0
			}), React.createElement("div", {
				id: "cover_url_drag_drop_pane",
				className: classNames("drop-pane", {
					active: this.state.cover_url_drop_active
				})
			})), React.createElement("div", {
				className: "drop-progress",
				style: {
					width: this.state.cover_url_drop_percentage + "%"
				}
			}), React.createElement("p", null, "poster_url:"), React.createElement("div", {
				className: "frame poster-drop"
			}, React.createElement("img", {
				className: "",
				src: this.state.hentai_video.poster_url || App.transparent,
				width: "100%"
			}), React.createElement("div", {
				id: "poster_url_drag_drop_pane",
				className: classNames("drop-pane", {
					active: this.state.poster_url_drop_active
				})
			})), React.createElement("div", {
				className: "drop-progress",
				style: {
					width: this.state.poster_url_drop_percentage + "%"
				}
			}), React.createElement("p", null, "sample_poster_url:"), React.createElement("div", {
				className: "frame"
			}, React.createElement("img", {
				className: "",
				src: this.state.hentai_video.sample_poster_url || App.transparent,
				width: "100%"
			}))), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-12 flex-row align-center"
			}, "Tags Search:", React.createElement("input", {
				type: "text",
				className: "",
				placeholder: "Tag search term (usually name of hentai)",
				value: this.state.hentai_video.tag_term,
				onChange: function(t) {
					e.updateField("tag_term", t.target.value)
				}
			}), React.createElement("strong", null, "slug:"), " ", React.createElement("input", {
				type: "text",
				className: "flex",
				placeholder: "Slug",
				value: this.state.hentai_video.slug,
				onChange: function(t) {
					e.updateField("slug", t.target.value)
				}
			}))), _.map(this.state.tag_search_results, function(t, a) {
				return React.createElement("section", {
					className: "row",
					key: a
				}, React.createElement("section", {
					className: "col-xs-3"
				}, React.createElement("button", {
					className: "btn btn-primary btn-shadow btn-sm",
					disabled: e.state.is_loading,
					onClick: function(t) {
						e.searchSites(t, a)
					}
				}, React.createElement("span", {
					className: "text"
				}, "Search ", a))), React.createElement("section", {
					className: "col-xs-9 flex-col tse-scrollable"
				}, React.createElement("div", {
					className: "tse-content"
				}, _.map(e.state.tag_search_results[a], function(t, n) {
					return React.createElement("div", {
						className: classNames("tag-search-result", {
							active: e.state.selected_tag_search_results[a] == t
						}),
						key: n,
						onClick: function(n) {
							e.toggleTagSearchResult(n, a, t)
						}
					}, React.createElement("div", null, t.title, " - (", t.tags.length, " tags)"), e.state.selected_tag_search_results.hh == t ? React.createElement("div", {
						className: "flex-col"
					}, _.map(t.tags, function(e, t) {
						return React.createElement("span", {
							key: t,
							className: "tag"
						}, e)
					})) : null)
				}))))
			}), React.createElement("section", {
				className: "row"
			}, React.createElement("section", {
				className: "col-xs-5"
			}, "tags (manual):", React.createElement("textarea", {
				className: "description-input",
				value: this.state.hentai_video.manual_tags,
				onChange: function(t) {
					e.updateField("manual_tags", t.target.value)
				}
			}), React.createElement("button", {
				className: "btn btn-primary btn-shadow btn-sm",
				disabled: this.state.is_loading || !this.state.hentai_video.id,
				onClick: this.commitManual
			}, React.createElement("span", {
				className: "text"
			}, "Create Hentai Video"))))))))
		};
		var s = a(1),
			i = n(s),
			r = a(24),
			o = n(r),
			c = a(26),
			l = n(c),
			u = a(4),
			d = n(u)
	}, 
	
	
	
	
	
	
	
	
	
	
	
	function(e, t, a) {
		"use strict";

		function n(e) {
			return e && e.__esModule ? e : {
				"default": e
			}
		}
		Object.defineProperty(t, "__esModule", {
			value: !0
		});
		
	

		
		var i = a(7),
			r = n(i),
			o = a(28),
			c = n(o),
			l = a(2),
			u = n(l),
			d = a(3),
			p = n(d),
			h = a(6),
			m = n(h),
			f = a(5),
			v = n(f),
			g = a(8),
			y = n(g),
			b = a(4),
			E = n(b),
			w = a(1),
			R = n(w)
	}, function(e, t, a) {
		var n = {
			EventEmitter: a(37)
		};
		e.exports = n
	}, function(e, t, a) {
		(function(t) {
			"use strict";

			function n(e, t) {
				if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
			}
			var s = a(38),
				i = a(40),
				r = a(41),
				o = a(20),
				c = function() {
					function e() {
						n(this, e), this._subscriber = new i, this._currentSubscription = null
					}
					return e.prototype.addListener = function(e, t, a) {
						return this._subscriber.addSubscription(e, new s(this._subscriber, t, a))
					}, e.prototype.once = function(e, t, a) {
						var n = this;
						return this.addListener(e, function() {
							n.removeCurrentListener(), t.apply(a, arguments)
						})
					}, e.prototype.removeAllListeners = function(e) {
						this._subscriber.removeAllSubscriptions(e)
					}, e.prototype.removeCurrentListener = function() {
						this._currentSubscription ? void 0 : "production" !== t.env.NODE_ENV ? o(!1, "Not in an emitting cycle; there is no current subscription") : o(!1), this._subscriber.removeSubscription(this._currentSubscription)
					}, e.prototype.listeners = function(e) {
						var t = this._subscriber.getSubscriptionsForType(e);
						return t ? t.filter(r.thatReturnsTrue).map(function(e) {
							return e.listener
						}) : []
					}, e.prototype.emit = function(e) {
						var t = this._subscriber.getSubscriptionsForType(e);
						if (t) {
							for (var a = Object.keys(t), n = 0; n < a.length; n++) {
								var s = a[n],
									i = t[s];
								i && (this._currentSubscription = i, this.__emitToSubscription.apply(this, [i].concat(Array.prototype.slice.call(arguments))))
							}
							this._currentSubscription = null
						}
					}, e.prototype.__emitToSubscription = function(e, t) {
						var a = Array.prototype.slice.call(arguments, 2);
						e.listener.apply(e.context, a)
					}, e
				}();
			e.exports = c
		}).call(t, a(9))
	}, function(e, t, a) {
		"use strict";

		function n(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}

		function s(e, t) {
			if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function, not " + typeof t);
			e.prototype = Object.create(t && t.prototype, {
				constructor: {
					value: e,
					enumerable: !1,
					writable: !0,
					configurable: !0
				}
			}), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
		}
		var i = a(39),
			r = function(e) {
				function t(a, s, i) {
					n(this, t), e.call(this, a), this.listener = s, this.context = i
				}
				return s(t, e), t
			}(i);
		e.exports = r
	}, function(e, t) {
		"use strict";

		function a(e, t) {
			if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
		}
		var n = function() {
			function e(t) {
				a(this, e), this.subscriber = t
			}
			return e.prototype.remove = function() {
				this.subscriber && (this.subscriber.removeSubscription(this), this.subscriber = null)
			}, e
		}();
		e.exports = n
	}, function(e, t, a) {
		(function(t) {
			"use strict";

			function n(e, t) {
				if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
			}
			var s = a(20),
				i = function() {
					function e() {
						n(this, e), this._subscriptionsForType = {}, this._currentSubscription = null
					}
					return e.prototype.addSubscription = function(e, a) {
						a.subscriber !== this ? "production" !== t.env.NODE_ENV ? s(!1, "The subscriber of the subscription is incorrectly set.") : s(!1) : void 0, this._subscriptionsForType[e] || (this._subscriptionsForType[e] = []);
						var n = this._subscriptionsForType[e].length;
						return this._subscriptionsForType[e].push(a), a.eventType = e, a.key = n, a
					}, e.prototype.removeAllSubscriptions = function(e) {
						void 0 === e ? this._subscriptionsForType = {} : delete this._subscriptionsForType[e]
					}, e.prototype.removeSubscription = function(e) {
						var t = e.eventType,
							a = e.key,
							n = this._subscriptionsForType[t];
						n && delete n[a]
					}, e.prototype.getSubscriptionsForType = function(e) {
						return this._subscriptionsForType[e]
					}, e
				}();
			e.exports = i
		}).call(t, a(9))
	}, function(e, t) {
		"use strict";

		function a(e) {
			return function() {
				return e
			}
		}

		function n() {}
		n.thatReturns = a, n.thatReturnsFalse = a(!1), n.thatReturnsTrue = a(!0), n.thatReturnsNull = a(null), n.thatReturnsThis = function() {
			return this
		}, n.thatReturnsArgument = function(e) {
			return e
		}, e.exports = n
	}]);

}
